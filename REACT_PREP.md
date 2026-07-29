# React Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of React interview questions — from fundamentals to advanced architecture — with clear answers and code examples where they help. Covers React 18/19. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions)
- [React Basics](#react-basics)
- [Hooks](#hooks)
- [Component Patterns](#component-patterns)
- [State Management](#state-management)
- [Performance Optimization](#performance-optimization)
- [React Router](#react-router)
- [Forms & Validation](#forms-validation)
- [Testing](#testing)
- [React 18+ Features](#react-18-features)
- [Advanced / Architecture](#advanced-architecture)
- [Common Coding Challenges](#common-coding-challenges)
- [Behavioral / Scenario-Based Questions](#behavioral-scenario-questions)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="most-asked-tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every React interview. If you're short on time, start here.

### Q: What is the difference between useEffect and useLayoutEffect?
**Answer:** Both run side effects, but timing differs. `useEffect` runs asynchronously *after* the browser has painted the screen, so it never blocks visual updates. `useLayoutEffect` runs synchronously *after* DOM mutations but *before* the browser paints, so it can block painting. Use `useLayoutEffect` only when you need to measure or adjust the DOM before the user sees a flicker (e.g., positioning a tooltip based on element size). For everything else — fetching data, subscriptions, logging — use `useEffect`.

### Q: Why do we need keys when rendering lists in React?
**Answer:** Keys help React identify which items were added, removed, or changed during reconciliation. Without stable keys, React can misattribute state or reorder DOM nodes incorrectly — for example, an input's typed value ending up on the wrong row after a reorder. Keys should be stable, unique identifiers from your data (like a database `id`), not array indexes, especially if the list can be reordered, filtered, or edited in the middle.

### Q: What is the difference between controlled and uncontrolled components?
**Answer:** A controlled component's value lives in React state — you set `value` and update it via `onChange`, making React the single source of truth. An uncontrolled component keeps its own state internally in the DOM, and you read it only when needed via a `ref`. Controlled gives you more control (validation, conditional formatting) at the cost of more code; uncontrolled is simpler for basic cases like a file input or quick integrations with non-React code.

**Example:**
```jsx
// Controlled
<input value={name} onChange={e => setName(e.target.value)} />

// Uncontrolled
<input ref={inputRef} defaultValue="Asha" />
```

### Q: What actually happens when you call a state setter (e.g., setCount)?
**Answer:** Calling a state setter schedules a re-render — it doesn't update the value immediately. React marks the component as needing an update, then re-runs the component function with the new state on the next render pass. Multiple setter calls inside the same event handler are batched into a single re-render. This is why logging the state variable right after calling its setter still shows the old value.

### Q: Why shouldn't you mutate state directly in React?
**Answer:** React often relies on reference comparison (not deep comparison) to detect changes — this is central to how `React.memo` and dependency arrays work. If you mutate an array or object directly (e.g., `state.items.push(x)`), the reference stays the same, so React may not realize anything changed and won't re-render. Always create a new object or array (spread syntax, `.map()`, `.filter()`, etc.) so React can see the update.

### Q: What is the difference between props and state?
**Answer:** Props are read-only data passed down from a parent — a child can't modify its own props. State is data a component owns and manages internally, which can change over time and triggers a re-render on update. Props flow down through the tree; state is local to the component that declares it (unless lifted up or shared globally).

### Q: What are the Rules of Hooks and why do they matter?
**Answer:** Only call Hooks at the top level of a function — never inside loops, conditions, or nested functions — and only from React function components or custom Hooks. React relies on the *order* Hooks are called in to correctly match state between renders; if that order changes between renders, React can no longer reliably tell which `useState` call owns which piece of state.

### Q: What is the Virtual DOM?
**Answer:** The Virtual DOM is a lightweight JavaScript representation of the real DOM. When state changes, React builds a new Virtual DOM tree, diffs it against the previous one, and computes the minimal set of real DOM operations needed — then applies only those changes. This avoids expensive, full-page DOM manipulation on every update.

### Q: What is the difference between useMemo and useCallback?
**Answer:** Both memoize something, but `useMemo` memoizes a computed *value*, while `useCallback` memoizes a *function reference*. In fact, `useCallback(fn, deps)` is essentially shorthand for `useMemo(() => fn, deps)`. Use `useMemo` for expensive calculations you don't want to redo every render; use `useCallback` when passing a stable function reference to a child (especially one wrapped in `React.memo`) to avoid breaking its memoization.

### Q: What causes unnecessary re-renders, and how do you prevent them?
**Answer:** Common causes: a parent re-rendering and passing new object/array/function references as props each time, a Context value changing and re-rendering every consumer, or state living higher in the tree than it needs to. Prevent them with `React.memo` (skip re-render if props are shallowly equal), `useMemo`/`useCallback` (keep references stable), splitting large contexts into smaller ones, and keeping state as local as possible.

### Q: What's the difference between React.memo and useMemo?
**Answer:** `React.memo` is a higher-order component that wraps an entire component and skips re-rendering it if its props haven't changed. `useMemo` is a hook used *inside* a component to avoid recalculating an expensive value on every render. Same underlying idea — avoid repeated work — applied at the component level vs. the value level.

### Q: What happens with different useEffect dependency arrays?
**Answer:** No array → the effect runs after every render. Empty array `[]` → it runs once, right after the initial mount. Array with values `[a, b]` → it runs after mount and again whenever `a` or `b` changes between renders. Leaving out a value the effect actually uses is a very common source of bugs (stale closures).

### Q: What is a stale closure in React, and how do you fix it?
**Answer:** A stale closure happens when a function — an effect, a callback, a timer — captures a variable's value from a previous render and keeps using that old value, because JavaScript closures capture variables at creation time. It usually shows up when a `useEffect` or `useCallback` references state but omits it from the dependency array. Fix it by adding the correct dependencies, using the functional updater form (`setCount(c => c + 1)`), or storing the latest value in a ref.

### Q: useState vs useRef — why doesn't updating a ref cause a re-render?
**Answer:** `useState` triggers a re-render whenever its setter is called, because React needs to reflect the new value in the UI. `useRef` returns a mutable object (`{ current: value }`) that persists across renders, but changing `.current` does **not** trigger a re-render — it's meant for values you need to keep around (a DOM node, a timer ID, a previous value) without affecting what's rendered.

### Q: Why is the functional updater form (prevState => newState) recommended?
**Answer:** When a new state value depends on the previous one, the functional form guarantees you're working with the most current state — even if multiple updates happen in the same batch. Using the plain-value form (`setCount(count + 1)`) can read a stale `count` from the closure if called more than once before the next re-render.

**Example:**
```jsx
// Risky if called multiple times before re-render
setCount(count + 1);

// Always correct
setCount(prev => prev + 1);
```

---

<a id="react-basics"></a>
## React Basics

### Q: What is JSX?
**Answer:** JSX (JavaScript XML) is a syntax extension that lets you write HTML-like markup directly inside JavaScript. Browsers don't understand it directly — a tool like Babel compiles it into `React.createElement()` calls that produce plain JavaScript objects describing what should appear on screen.

**Example:**
```jsx
const element = <h1>Hello, world!</h1>;
// Compiles roughly to:
const element = React.createElement('h1', null, 'Hello, world!');
```

### Q: What is the difference between an element and a component?
**Answer:** A React element is a plain, immutable JavaScript object describing what you want to see (a type, props, and children) — cheap to create. A component is a function or class that returns elements based on props/state. You render components; they produce elements, which React uses to build and update the actual DOM.

### Q: What is a React component? Functional vs. class components?
**Answer:** A component is a reusable, self-contained piece of UI. Functional components are plain JavaScript functions that accept props and return JSX; with Hooks, they can also hold state and run side effects. Class components extend `React.Component`, use `this.state`/`this.setState()`, and have lifecycle methods. Functional components with Hooks are the modern standard; class components mostly appear in legacy code.

**Example:**
```jsx
// Functional
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

// Class
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

### Q: What are props?
**Answer:** Props ("properties") are read-only inputs passed from a parent component to a child, similar to function arguments. They customize how a component renders and behaves. A child can never modify its own props.

**Example:**
```jsx
function Greeting({ name }) {
  return <p>Hello, {name}!</p>;
}
// Usage: <Greeting name="Asha" />
```

### Q: What is state in React?
**Answer:** State is data a component owns and manages internally. It can change over time (usually due to user interaction), and updating it triggers a re-render so the UI reflects the new value. Unlike props, state is private to the component unless it's lifted up or shared.

**Example:**
```jsx
function Counter() {
  const [count, setCount] = useState(0);
  return <button onClick={() => setCount(count + 1)}>{count}</button>;
}
```

### Q: What are the key differences between props and state?
**Answer:** Props come from a parent and are read-only from the child's perspective; state is owned and updated internally by the component itself. Changing props re-renders a component "from the outside" (the parent re-renders and passes new props down); changing state re-renders it "from the inside." Both can trigger re-renders, but ownership and mutability differ.

### Q: What are the lifecycle methods in class components?
**Answer:** The three broad phases are Mounting, Updating, and Unmounting. Key methods: `constructor()` for setup, `render()` returns JSX, `componentDidMount()` runs once after the first render (good for data fetching), `componentDidUpdate(prevProps, prevState)` runs after updates (good for reacting to changes), and `componentWillUnmount()` runs cleanup before removal (clearing timers/subscriptions).

### Q: How do class lifecycle methods map to Hooks?
**Answer:** `componentDidMount` ≈ `useEffect(() => {...}, [])`. `componentDidUpdate` ≈ `useEffect(() => {...}, [dep1, dep2])`. `componentWillUnmount` ≈ the cleanup function returned from `useEffect`. It's not a perfect 1:1 mapping — Hooks group logic by *concern* rather than by lifecycle phase — but this mental model covers most cases.

### Q: How does React's one-way (unidirectional) data flow work?
**Answer:** Data flows in a single direction: from parent to child via props. A child can't directly change data owned by its parent — instead, the parent typically passes a callback prop that the child calls to *request* a change, and the parent updates its own state, which flows back down as new props. This makes apps more predictable and easier to debug than two-way binding.

### Q: How do you render a list of items in React?
**Answer:** Use JavaScript's `Array.prototype.map()` inside JSX to turn an array of data into an array of elements, giving each item a unique, stable `key`.

**Example:**
```jsx
function List({ items }) {
  return (
    <ul>
      {items.map(item => (
        <li key={item.id}>{item.name}</li>
      ))}
    </ul>
  );
}
```

### Q: What is prop drilling?
**Answer:** Prop drilling is passing data through several layers of nested components — even ones that don't need it themselves — just so a deeply nested child can access it. It makes code harder to maintain and refactor. Common fixes: the Context API, or a state management library like Redux or Zustand.

### Q: What are React Fragments, and why use them instead of a wrapper div?
**Answer:** A component can only return a single root node from `render()`. Fragments (`<>...</>` or `<React.Fragment>...</React.Fragment>`) let you group multiple children without adding an extra node to the real DOM — useful when a wrapping `<div>` would break styling (e.g., inside a `<table>`) or add meaningless nesting.

**Example:**
```jsx
function Row() {
  return (
    <>
      <td>Cell 1</td>
      <td>Cell 2</td>
    </>
  );
}
```

---

<a id="hooks"></a>
## Hooks

### Q: What is useState and how do you use it?
**Answer:** `useState` is a Hook that lets a function component hold and update local state. It returns a pair: the current value, and a function to update it. Calling the updater schedules a re-render with the new value.

**Example:**
```jsx
const [count, setCount] = useState(0);
```

### Q: What is useEffect and what problem does it solve?
**Answer:** `useEffect` lets you run side effects — data fetching, subscriptions, timers, manual DOM changes — in function components. It replaces the need for `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` from class components.

**Example:**
```jsx
useEffect(() => {
  const id = setInterval(() => console.log('tick'), 1000);
  return () => clearInterval(id); // cleanup
}, []);
```

### Q: Explain the different forms of the useEffect dependency array.
**Answer:** No array runs the effect after every render. `[]` runs it once, after the initial mount only. `[a, b]` runs it after mount and again whenever `a` or `b` changes. The cleanup function (returned from the effect) runs before the effect re-runs, and again when the component unmounts.

**Example:**
```jsx
useEffect(() => { console.log('every render'); });
useEffect(() => { console.log('once on mount'); }, []);
useEffect(() => { console.log('when userId changes'); }, [userId]);
```

### Q: What is useContext and what problem does it solve?
**Answer:** `useContext` lets a component read a value from the nearest matching `Context.Provider` above it in the tree, without passing that value down manually through every intermediate component — avoiding prop drilling.

**Example:**
```jsx
const ThemeContext = React.createContext('light');

function ThemedButton() {
  const theme = useContext(ThemeContext);
  return <button className={theme}>Click</button>;
}
```

### Q: What is useRef and what are its common use cases?
**Answer:** `useRef` returns a mutable object with a `.current` property that persists across renders without causing a re-render when it changes. Common uses: directly accessing/manipulating a DOM node (e.g., focusing an input), storing a mutable value that shouldn't trigger a re-render (a timer ID, a previous value), and holding instance-like variables in function components.

**Example:**
```jsx
function TextInput() {
  const inputRef = useRef(null);
  useEffect(() => { inputRef.current.focus(); }, []);
  return <input ref={inputRef} />;
}
```

### Q: What is useMemo and when should you use it?
**Answer:** `useMemo` memoizes the result of an expensive calculation so it's only recomputed when a dependency changes, instead of on every render. Reach for it when profiling shows a genuine cost — overusing it for cheap computations just adds complexity without benefit.

**Example:**
```jsx
const sortedList = useMemo(() => expensiveSort(items), [items]);
```

### Q: What is useCallback and when should you use it?
**Answer:** `useCallback` returns a memoized version of a function that only changes if one of its dependencies changes. It's most useful when passing callbacks to children wrapped in `React.memo`, or as a dependency of another hook, so a new function reference doesn't trigger unnecessary re-renders or effect re-runs.

**Example:**
```jsx
const handleClick = useCallback(() => {
  doSomething(id);
}, [id]);
```

### Q: What is useReducer and when would you use it instead of useState?
**Answer:** `useReducer` manages state with a reducer function — `(state, action) => newState` — similar to Redux's pattern. Prefer it over `useState` when you have complex state logic with multiple sub-values, when the next state depends heavily on the previous one, or when several related event handlers update state in similar ways — it keeps the update logic centralized and predictable.

**Example:**
```jsx
function reducer(state, action) {
  switch (action.type) {
    case 'increment': return { count: state.count + 1 };
    case 'decrement': return { count: state.count - 1 };
    default: return state;
  }
}
const [state, dispatch] = useReducer(reducer, { count: 0 });
```

### Q: What are the Rules of Hooks?
**Answer:** Only call Hooks at the top level — never inside loops, conditions, or nested functions — so React can reliably match state to the same call in the same order every render. And only call Hooks from React function components or other custom Hooks, never from plain JS functions. `eslint-plugin-react-hooks` enforces both rules automatically.

### Q: How do you write a custom hook? Give an example.
**Answer:** A custom hook is just a JavaScript function whose name starts with `use` and that can call other Hooks internally. It lets you extract and reuse stateful logic between components without changing your component hierarchy — unlike HOCs or render props.

**Example:**
```jsx
function useWindowWidth() {
  const [width, setWidth] = useState(window.innerWidth);
  useEffect(() => {
    const handleResize = () => setWidth(window.innerWidth);
    window.addEventListener('resize', handleResize);
    return () => window.removeEventListener('resize', handleResize);
  }, []);
  return width;
}
```

### Q: What is useLayoutEffect and when should you use it over useEffect?
**Answer:** `useLayoutEffect` fires synchronously after DOM mutations but before the browser paints, letting you measure and adjust layout before the user sees anything — avoiding visual flicker. Use it sparingly, e.g., measuring an element to position a tooltip. Everything else should use `useEffect`, which doesn't block painting.

### Q: What is useImperativeHandle?
**Answer:** `useImperativeHandle` customizes the instance value exposed to a parent when it attaches a `ref` to a child wrapped in `forwardRef`. It lets a child expose only specific methods to the parent — like `focus()` or `reset()` — instead of the whole DOM node.

**Example:**
```jsx
const FancyInput = forwardRef((props, ref) => {
  const inputRef = useRef();
  useImperativeHandle(ref, () => ({
    focus: () => inputRef.current.focus(),
  }));
  return <input ref={inputRef} />;
});
```

---

<a id="component-patterns"></a>
## Component Patterns

### Q: What is a Higher-Order Component (HOC)?
**Answer:** An HOC is a function that takes a component and returns a new, enhanced component — adding shared behavior (data fetching, auth checks) without modifying the original. Convention names them `withSomething`.

**Example:**
```jsx
function withLoading(Component) {
  return function Wrapped({ isLoading, ...props }) {
    if (isLoading) return <p>Loading...</p>;
    return <Component {...props} />;
  };
}
```

### Q: What is the render props pattern?
**Answer:** A render prop is a technique where a component accepts a function as a prop (often called `render` or `children`) and calls it to determine what to render, passing along internal state or data. It shares logic between components, similar in goal to HOCs and custom hooks.

**Example:**
```jsx
function MouseTracker({ render }) {
  const [pos, setPos] = useState({ x: 0, y: 0 });
  return (
    <div onMouseMove={e => setPos({ x: e.clientX, y: e.clientY })}>
      {render(pos)}
    </div>
  );
}
// Usage: <MouseTracker render={pos => <p>{pos.x}, {pos.y}</p>} />
```

### Q: What are compound components?
**Answer:** Compound components are a pattern where several components work together to form one cohesive UI, sharing implicit state (often via Context) while letting the consumer control structure and composition — similar to how native `<select>` and `<option>` work together.

**Example:**
```jsx
<Tabs>
  <Tabs.List>
    <Tabs.Tab index={0}>One</Tabs.Tab>
    <Tabs.Tab index={1}>Two</Tabs.Tab>
  </Tabs.List>
  <Tabs.Panels>
    <Tabs.Panel index={0}>Content One</Tabs.Panel>
    <Tabs.Panel index={1}>Content Two</Tabs.Panel>
  </Tabs.Panels>
</Tabs>
```

### Q: What does controlled vs. uncontrolled mean for custom components (beyond form inputs)?
**Answer:** The idea isn't limited to `<input>`. Any component can be controlled — the parent fully owns the state and passes it via props plus a change callback — or uncontrolled — the component manages its own internal state, optionally seeded by a `defaultValue`-style prop. Controlled gives the parent full coordination and a single source of truth; uncontrolled is simpler but harder to sync with other UI.

### Q: What is a Pure Component, and how does it relate to React.memo?
**Answer:** `React.PureComponent` (class components) automatically implements `shouldComponentUpdate` with a shallow prop/state comparison, skipping re-renders when nothing relevant changed. `React.memo` is the function-component equivalent — it wraps a component and skips re-rendering if props are shallowly equal to the previous render.

### Q: What is the Container/Presentational pattern?
**Answer:** This pattern splits components into "containers" (handle data fetching, state, and logic) and "presentational" components (purely receive props and render UI, no business logic). It improves reusability and testability — though with Hooks, this separation is now often achieved with custom hooks instead of dedicated container components.

### Q: HOCs vs. render props vs. custom hooks — when would you use which?
**Answer:** All three share reusable logic across components. Custom Hooks are the modern default — simplest syntax, no extra wrapper nesting, fully composable. HOCs and render props predate Hooks and still show up in older codebases or certain libraries, but for new code, custom Hooks are usually preferred unless you specifically need to wrap or inject rendering output, which Hooks alone can't do.

### Q: What is the Provider pattern?
**Answer:** The Provider pattern uses `<Context.Provider>` to make a value — state, functions, theme, etc. — available to any descendant that needs it, without prop drilling. It's the foundation many state-management and theming libraries build on to expose data throughout an app.

### Q: What does "composition over inheritance" mean in React?
**Answer:** React strongly favors composition — building complex components by combining smaller ones, including passing components as props or children — over class inheritance to share behavior. The React docs specifically recommend composition (via `children`/props) instead of building component inheritance hierarchies.

**Example:**
```jsx
function Card({ children }) {
  return <div className="card">{children}</div>;
}
// Usage: <Card><h2>Title</h2><p>Body</p></Card>
```

### Q: What is the prop-getters / "headless" pattern, and where might you see it?
**Answer:** A more advanced, flexible-API pattern where a component or hook returns a set of props to spread onto whatever DOM elements the consumer renders — giving the consumer full control over markup while the hook manages behavior, state, and accessibility. Common in headless UI libraries like Downshift, Radix, and react-table.

---

<a id="state-management"></a>
## State Management

### Q: What is the Context API and when should you use it?
**Answer:** Context passes data through the component tree without manually threading props at every level. It's ideal for relatively low-frequency global data — theme, authenticated user, locale — things many components need but that don't change on every keystroke.

### Q: What are the downsides of Context API for frequently-changing state?
**Answer:** Every component consuming a Context re-renders whenever its value changes, even if it only cares about part of that value — there's no built-in selective subscription like Redux's selectors. For state that updates often or is read by only a few components, Context can cause more re-renders than a dedicated state library with fine-grained subscriptions.

### Q: What are the core principles of Redux?
**Answer:** (1) Single source of truth — the whole app's state lives in one store. (2) State is read-only — the only way to change it is by dispatching an action. (3) Changes are made with pure functions (reducers) — given the same state and action, a reducer always produces the same result, with no side effects.

### Q: What are actions, reducers, and the store in Redux?
**Answer:** An action is a plain object describing what happened, e.g. `{ type: 'INCREMENT' }`. A reducer is a pure function that takes the current state and an action and returns the next state. The store holds the state tree and lets you dispatch actions, subscribe to changes, and read state via `getState()`.

**Example:**
```js
function counterReducer(state = { count: 0 }, action) {
  switch (action.type) {
    case 'increment': return { count: state.count + 1 };
    default: return state;
  }
}
```

### Q: What is middleware in Redux, and what are common examples?
**Answer:** Middleware sits between dispatching an action and it reaching the reducer, adding cross-cutting behavior like logging or crash reporting, or handling async logic. `redux-thunk` lets action creators return functions (for async calls); `redux-saga` uses generator functions to manage complex async flows and side effects.

### Q: What is Zustand and how does it differ from Redux?
**Answer:** Zustand is a small, unopinionated state management library with a simple hook-based API — no providers, action types, or reducer boilerplate required. Compared to Redux, it has far less setup, no mandatory action/dispatch pattern, and built-in support for selective re-rendering via selectors.

**Example:**
```js
const useStore = create(set => ({
  count: 0,
  increment: () => set(state => ({ count: state.count + 1 })),
}));
```

### Q: What is Recoil, and what are atoms and selectors?
**Answer:** Recoil is a state management library from Meta built specifically for React, using fine-grained, subscribable units. An "atom" is a piece of state components can read and write directly — like a globally shared `useState`. A "selector" is a pure, derived value computed from atoms (or other selectors), similar to a computed property, and can also be asynchronous.

### Q: How do you decide between Context API and a dedicated state library?
**Answer:** Consider scale, update frequency, and tooling needs. For a small app or infrequently-changing global values (theme, auth), Context is enough. For complex state, frequent updates, or when you need dev tools like time-travel debugging, middleware, or fine-grained subscriptions to avoid over-rendering, reach for Redux, Zustand, or a similar library.

### Q: What's the difference between local, lifted, and global state?
**Answer:** Local state lives and is used inside a single component. Lifted state is moved up to the closest common ancestor of components that need to share it, then passed back down via props. Global state is accessible from anywhere in the app (via Context or a state library) — typically used for the logged-in user, theme, or app-wide settings.

### Q: What is the difference between Redux Toolkit (RTK) and "plain" Redux?
**Answer:** Redux Toolkit is the officially recommended way to write Redux today. It cuts boilerplate drastically — `createSlice` auto-generates action creators and types from your reducer functions — and uses Immer internally, so you can write "mutating" update logic that's actually applied immutably under the hood. It also bundles good defaults like DevTools support and `redux-thunk`.

---

<a id="performance-optimization"></a>
## Performance Optimization

### Q: What commonly causes unnecessary re-renders in React?
**Answer:** A parent re-rendering and cascading to children that don't need to update; passing new object/array/function literals as props on every render (breaking shallow-equality checks); a Context value changing and re-rendering every consumer; and state living higher in the tree than necessary, forcing large subtrees to re-render for a small, localized change.

### Q: How does React.memo help with performance?
**Answer:** `React.memo` wraps a function component and skips re-rendering it if its props are shallowly equal to the previous render. It pays off most for components that render often with unchanged props, or that are expensive to render — wrapping every component isn't automatically a win, since the comparison itself has a small cost.

### Q: When should you use useMemo instead of just recalculating every render?
**Answer:** Use it when a calculation is genuinely expensive — sorting/filtering large lists, heavy math — and you want to skip redoing it unless its dependencies changed. For cheap calculations, the overhead of comparing dependencies can outweigh the benefit, so profile before reaching for it by default.

### Q: What is code splitting, and how do you implement it in React?
**Answer:** Code splitting breaks your bundle into smaller chunks that load on demand instead of all at once, cutting initial load time. `React.lazy()` combined with `<Suspense>` lazily loads a component only when it's actually rendered.

**Example:**
```jsx
const Settings = React.lazy(() => import('./Settings'));

function App() {
  return (
    <Suspense fallback={<Spinner />}>
      <Settings />
    </Suspense>
  );
}
```

### Q: What is lazy loading, and where else is it used besides components?
**Answer:** Lazy loading defers loading a resource until it's actually needed. Besides `React.lazy` for components, it's commonly applied to images (loading only as they scroll into view), routes (loading a page's code only when navigated to), and large third-party libraries used on just one page.

### Q: What is list virtualization (windowing), and why is it needed?
**Answer:** Virtualization renders only the list items currently visible in the viewport (plus a small buffer) instead of the entire list, drastically cutting DOM node count for very long lists. Libraries like `react-window` and `react-virtualized` track scroll position and render a moving "window" of items.

### Q: How does the "key" prop affect list performance and correctness?
**Answer:** A correct, stable key (e.g., a database ID) lets React precisely match old and new items during reconciliation, reusing DOM nodes and component state instead of destroying and recreating them. Using array indexes as keys for lists that reorder, filter, or have items inserted/removed can make React match the wrong items — causing visual glitches, lost input state, and extra DOM work.

### Q: How do you avoid memory leaks caused by useEffect?
**Answer:** Always clean up subscriptions, timers, and event listeners in the function returned from `useEffect` — it runs before the effect re-runs and when the component unmounts. A common leak is updating state after an async request resolves for a component that already unmounted; guard against it with a mounted flag or an `AbortController`.

**Example:**
```jsx
useEffect(() => {
  let isMounted = true;
  fetchData().then(data => { if (isMounted) setData(data); });
  return () => { isMounted = false; };
}, []);
```

### Q: How do you profile a React app to find performance bottlenecks?
**Answer:** The React DevTools Profiler records renders and shows how long each component took and *why* it re-rendered (props changed, state changed, parent re-rendered), pinpointing expensive or unnecessary renders. Browser DevTools' Performance tab helps with broader JS/paint/layout bottlenecks beyond React's own rendering.

### Q: How would you optimize a search input that filters a large list as the user types?
**Answer:** Debounce the input so filtering only runs after the user pauses typing, rather than on every keystroke. Consider combining this with `useDeferredValue` (React 18+) to keep typing responsive while the filtered list update is deprioritized, and virtualize the results if the filtered list can still be long.

### Q: What is the difference between debouncing and throttling?
**Answer:** Debouncing delays execution until activity pauses — the function runs only after events stop firing for a set time (ideal for search-as-you-type). Throttling guarantees a function runs at most once per fixed interval no matter how often the event fires (ideal for scroll or resize handlers).

### Q: What is bundle-size optimization, and how does it relate to React performance?
**Answer:** Even a fast-rendering app feels slow if users must download a huge JS bundle first. Techniques include code splitting/lazy loading, tree-shaking unused code, analyzing bundle composition (e.g., `webpack-bundle-analyzer`), and avoiding large dependencies when a lighter alternative exists.

---

<a id="react-router"></a>
## React Router

### Q: What is React Router and why do we need it?
**Answer:** React Router is the standard library for client-side routing in React single-page apps. Since an SPA loads one HTML page, React Router intercepts URL changes and renders the right components without a full page reload — keeping the URL in sync with what's displayed while preserving app state.

### Q: What is the difference between BrowserRouter and HashRouter?
**Answer:** `BrowserRouter` uses the HTML5 History API for clean URLs (e.g., `/about`), but needs server configuration to serve `index.html` for every route so a refreshed deep link doesn't 404. `HashRouter` stores the route in the URL hash (`/#/about`), which never reaches the server, so it works without server setup but produces less clean URLs.

### Q: How do you define routes with React Router (v6+)?
**Answer:** Wrap routes in a `<Routes>` element containing individual `<Route path="..." element={<Component />} />` entries.

**Example:**
```jsx
<BrowserRouter>
  <Routes>
    <Route path="/" element={<Home />} />
    <Route path="/about" element={<About />} />
  </Routes>
</BrowserRouter>
```

### Q: How do you navigate programmatically?
**Answer:** Use the `useNavigate` hook, which returns a function you call to change routes in response to code — e.g., after a form submits or a login succeeds.

**Example:**
```jsx
const navigate = useNavigate();
function handleLogin() {
  navigate('/dashboard');
}
```

### Q: How do you read dynamic URL parameters?
**Answer:** Define a dynamic segment in the route path (e.g., `/users/:id`), then read it with `useParams`.

**Example:**
```jsx
<Route path="/users/:id" element={<UserProfile />} />

function UserProfile() {
  const { id } = useParams();
  return <p>User ID: {id}</p>;
}
```

### Q: How do you implement nested routes?
**Answer:** Nest `<Route>` elements, and render the matched child route inside the parent using `<Outlet />`, which acts as a placeholder for whichever nested route currently matches.

**Example:**
```jsx
<Route path="/dashboard" element={<DashboardLayout />}>
  <Route path="settings" element={<Settings />} />
  <Route path="profile" element={<Profile />} />
</Route>

function DashboardLayout() {
  return (
    <div>
      <Sidebar />
      <Outlet />
    </div>
  );
}
```

### Q: How would you implement a protected/private route?
**Answer:** Create a wrapper component that checks authentication state and either renders the intended content or redirects to a login page with `<Navigate />` if the user isn't authenticated.

**Example:**
```jsx
function ProtectedRoute({ isAuthenticated, children }) {
  if (!isAuthenticated) return <Navigate to="/login" replace />;
  return children;
}
```

### Q: What is the difference between <Link> and a regular <a> tag?
**Answer:** `<Link>` intercepts the click and updates the route using React Router's internal navigation (via the History API), avoiding a full page reload and preserving app state. A plain `<a>` tag triggers a full browser navigation, losing any in-memory React state.

### Q: How do you handle a 404 / "not found" page?
**Answer:** Add a catch-all route with a wildcard path (`path="*"`) as the last route — React Router matches it when nothing else does.

**Example:**
```jsx
<Routes>
  <Route path="/" element={<Home />} />
  <Route path="*" element={<NotFound />} />
</Routes>
```

### Q: How do you lazy-load routes for better performance?
**Answer:** Combine `React.lazy()` with `<Suspense>` around your routes, so each page's code downloads only when the user actually navigates there, reducing the initial bundle size.

**Example:**
```jsx
const About = React.lazy(() => import('./About'));

<Suspense fallback={<Spinner />}>
  <Routes>
    <Route path="/about" element={<About />} />
  </Routes>
</Suspense>
```

---

<a id="forms-validation"></a>
## Forms & Validation

### Q: How do you create a controlled form input in React?
**Answer:** Bind the input's `value` to a state variable and update that state in `onChange`, so React state is always the single source of truth for what's displayed.

**Example:**
```jsx
function NameForm() {
  const [name, setName] = useState('');
  return <input value={name} onChange={e => setName(e.target.value)} />;
}
```

### Q: How do you handle form submission in React?
**Answer:** Attach an `onSubmit` handler to the `<form>` element and call `event.preventDefault()` inside it to stop the browser's default full-page-reload submission, then run your own logic — validation, an API call, etc.

**Example:**
```jsx
function handleSubmit(e) {
  e.preventDefault();
  console.log('Submitting:', formData);
}
// <form onSubmit={handleSubmit}>...</form>
```

### Q: How do you handle multiple input fields with a single change handler?
**Answer:** Give each input a `name` attribute matching a key in your state object, then use that name to update the right field dynamically.

**Example:**
```jsx
function handleChange(e) {
  const { name, value } = e.target;
  setFormData(prev => ({ ...prev, [name]: value }));
}
```

### Q: How would you validate a form manually, without a library?
**Answer:** Run validation logic on change, on blur, or on submit, storing an `errors` object in state and conditionally rendering messages next to each field. On submit, check all fields and only proceed (e.g., call an API) if there are no errors.

### Q: What problem does Formik solve, and what are its core building blocks?
**Answer:** Formik removes the boilerplate of manually wiring up `value`, `onChange`, `onBlur`, and error state for every field. Its core pieces are `values`, `errors`, `touched`, handlers like `handleChange`/`handleBlur`/`handleSubmit`, plus integration with schema validation libraries like Yup.

### Q: How does React Hook Form differ from Formik?
**Answer:** React Hook Form registers inputs as uncontrolled by default (using refs) rather than storing every keystroke in React state, which significantly cuts re-renders for large forms and improves performance. It generally requires less code than Formik, and integrates with schema validators like Yup or Zod through resolvers.

**Example:**
```jsx
const { register, handleSubmit } = useForm();
// <form onSubmit={handleSubmit(onSubmit)}><input {...register('email')} /></form>
```

### Q: Should you validate on every keystroke, on blur, or on submit?
**Answer:** It's a UX trade-off. Validating every keystroke gives the fastest feedback but can feel naggy on fields the user hasn't finished typing (e.g., flagging an "invalid email" mid-type). A common pattern: hold off showing errors until the first blur or submit attempt, then re-validate on change afterward for instant feedback as the user fixes it.

### Q: How do you handle file uploads in a React form?
**Answer:** Use an uncontrolled `<input type="file">` (file inputs can't really be "controlled" the normal way), read the selected file(s) from `event.target.files`, and typically send them via `FormData` in a fetch/axios request rather than JSON.

**Example:**
```jsx
function handleFileChange(e) {
  const file = e.target.files[0];
  const formData = new FormData();
  formData.append('file', file);
}
```

### Q: How would you implement a debounced search/autocomplete field?
**Answer:** Store the input value in state as usual, but delay the actual search/API call — using `setTimeout` inside a `useEffect`, or a debounce utility — until the user pauses typing for a short interval, cancelling any pending timer if the value changes again first.

**Example:**
```jsx
useEffect(() => {
  const timer = setTimeout(() => search(query), 300);
  return () => clearTimeout(timer);
}, [query]);
```

### Q: How do you reset a form after successful submission?
**Answer:** With plain state, reset by setting it back to its initial values (`setFormData(initialState)`). With React Hook Form, call the `reset()` function returned by `useForm()`. With an uncontrolled form using refs, call `formRef.current.reset()`.

---

<a id="testing"></a>
## Testing

### Q: Why do we test React components?
**Answer:** Tests catch regressions before they reach users, document expected behavior, and give the confidence to refactor or upgrade dependencies without manually re-checking every feature by hand. For UI specifically, they also confirm components render correctly and respond properly to user interaction.

### Q: What is Jest, and what role does it play in testing React apps?
**Answer:** Jest is a JavaScript testing framework — it provides the test runner, the assertion library (`expect`), and mocking utilities. It's commonly paired with React Testing Library, which adds utilities specifically for rendering and interacting with React components inside tests.

### Q: What is React Testing Library (RTL), and what's its guiding philosophy?
**Answer:** RTL's philosophy is "test your software the way users use it" — instead of checking internal component state or implementation details, you query the rendered output the way a user would (visible text, labels, roles) and simulate real interactions. This makes tests more resilient to internal refactors that don't change user-facing behavior.

**Example:**
```jsx
import { render, screen, fireEvent } from '@testing-library/react';

test('increments counter on click', () => {
  render(<Counter />);
  fireEvent.click(screen.getByText('Increment'));
  expect(screen.getByText('Count: 1')).toBeInTheDocument();
});
```

### Q: What's the difference between shallow rendering and full DOM rendering?
**Answer:** Shallow rendering (historically via Enzyme) renders only one level deep, stubbing out child components — useful for isolated unit tests but can miss integration issues. Full DOM rendering (RTL's default, via jsdom) renders the whole component tree, closer to what actually happens in a browser, which is why it's generally preferred today.

### Q: How do you test a component that fetches data?
**Answer:** Mock the network request — with `jest.mock`, Mock Service Worker (`msw`), or by mocking `fetch`/axios directly — so the test doesn't depend on a real API, then assert the component shows a loading state initially and the fetched data afterward, typically using RTL's `findBy*` queries, which wait for async updates.

### Q: How do you simulate user events in tests?
**Answer:** `@testing-library/user-event` simulates real user interactions — typing, clicking, tabbing — more realistically than the lower-level `fireEvent` (e.g., `userEvent.type()` fires the full sequence of keydown/keypress/input/keyup events per character).

**Example:**
```jsx
import userEvent from '@testing-library/user-event';
await userEvent.type(screen.getByRole('textbox'), 'hello');
```

### Q: How do you test a custom hook in isolation?
**Answer:** Use `renderHook` from `@testing-library/react`, which renders the hook inside a minimal test component and gives you access to its return value plus a way to trigger updates via `act()`.

**Example:**
```jsx
const { result } = renderHook(() => useCounter());
act(() => result.current.increment());
expect(result.current.count).toBe(1);
```

### Q: What is snapshot testing, and what are its pros and cons?
**Answer:** Snapshot testing renders a component, serializes the output, and saves it to a file; future runs compare current output against the saved snapshot and fail on unexpected changes. Pros: catches unintended UI changes with almost no effort. Cons: snapshots can get large and noisy, and developers often blindly "update" failing snapshots without reviewing the diff, which erodes their value.

### Q: What's the difference between a mock, a stub, and a spy?
**Answer:** A stub is a fake implementation returning canned data, used to isolate the code under test. A spy wraps a real (or fake) function to record how it was called — arguments, call count — while optionally still calling through to the original. "Mock" is often used loosely for either, but strictly refers to an object pre-programmed with expectations about how it should be called, which can fail the test if those expectations aren't met.

### Q: What is code coverage, and what are its limitations as a quality metric?
**Answer:** Code coverage measures what percentage of your code executes during your test suite — statements, branches, functions, lines. High coverage doesn't guarantee correctness, since a test can execute a line without meaningfully asserting on its behavior. It's a useful signal for finding untested code, but shouldn't be treated as a target to game.

---

<a id="react-18-features"></a>
## React 18+ Features

### Q: What is concurrent rendering in React 18?
**Answer:** Concurrent rendering lets React prepare multiple versions of the UI at once and interrupt, pause, or abandon a render in progress if something more urgent comes in — like user input — instead of committing to one synchronous render that blocks the main thread until it finishes. It's the underlying capability that `useTransition`, `useDeferredValue`, and streaming SSR build on, opted into via the new root API.

### Q: What is automatic batching in React 18?
**Answer:** Before React 18, React only batched multiple state updates inside its own event handlers into one re-render. React 18 extends batching to updates inside promises, `setTimeout`, native event handlers, and anywhere else — so several `setState` calls anywhere are grouped into a single re-render by default.

**Example:**
```jsx
setTimeout(() => {
  setCount(c => c + 1);
  setFlag(f => !f);
  // React 18: still just one re-render, even inside setTimeout
}, 1000);
```

### Q: What is the useTransition hook?
**Answer:** `useTransition` lets you mark a state update as a low-priority "transition," so React keeps the UI responsive to more urgent updates (like typing) while the transition happens in the background — and can show a pending indicator while it's in progress.

**Example:**
```jsx
const [isPending, startTransition] = useTransition();
function handleChange(e) {
  setInput(e.target.value); // urgent
  startTransition(() => {
    setResults(filterList(e.target.value)); // low-priority
  });
}
```

### Q: What is useDeferredValue, and how does it differ from useTransition?
**Answer:** `useDeferredValue` gives you a "lagged" version of a value that updates at lower priority, letting you defer re-rendering an expensive part of the UI without controlling the state update itself — useful when you don't own the `setState` call (e.g., a value passed in via props). `useTransition` instead wraps the state update itself as low-priority. Different angles on the same underlying problem.

### Q: How has Suspense evolved in React 18?
**Answer:** Suspense originally supported code-splitting via `React.lazy`. React 18 expands it toward data fetching (in frameworks built to support it) and enables streaming server-side rendering, where the server sends HTML for ready parts of the page immediately and streams in slower parts as they become ready, hydrating each piece as it arrives.

### Q: What changed with the root API in React 18?
**Answer:** React 18 introduces `createRoot` (from `react-dom/client`) to replace the legacy `ReactDOM.render()`. Using `createRoot` opts your app into the new concurrent features; apps still calling the old `ReactDOM.render` keep the previous, non-concurrent behavior even when running React 18.

**Example:**
```jsx
import { createRoot } from 'react-dom/client';
const root = createRoot(document.getElementById('root'));
root.render(<App />);
```

### Q: What is streaming SSR, and why does it matter?
**Answer:** Streaming server-side rendering sends the HTML response in chunks as it's generated, instead of waiting for the whole page to be ready. Paired with Suspense, slower parts of a page (e.g., a component waiting on data) can stream in later without blocking the initial HTML — improving perceived performance and time-to-first-byte.

### Q: What is the useId hook, and why was it added?
**Answer:** `useId` generates a stable, unique ID that stays consistent between server and client rendering — important for accessibility attributes like linking a `<label>` to an `<input>` via matching IDs. Randomly-generated server IDs previously risked mismatching the client's IDs during hydration.

### Q: What's new in React 19 that builds on React 18 (Actions, the use hook)?
**Answer:** React 19 introduced Actions — functions that handle async transitions like form submissions, with built-in pending/error state via hooks like `useActionState` and `useFormStatus` — the `use` hook for reading promises or context conditionally during render, and `useOptimistic` for showing an optimistic UI state while an async update is in flight.

### Q: What are React Server Components (RSC), conceptually?
**Answer:** Server Components render entirely on the server and send a serialized description to the client, never shipping their own JavaScript to the browser bundle — reducing bundle size and allowing direct server-side data access (e.g., querying a database inside the component). They're combined with regular Client Components, which still render and hydrate in the browser for interactivity — a hybrid model popularized by frameworks like Next.js's App Router.

---

<a id="advanced-architecture"></a>
## Advanced / Architecture

### Q: How does reconciliation actually work under the hood?
**Answer:** On each update, React builds a new Virtual DOM tree and compares it to the previous one using a heuristic diffing algorithm — not a full generic tree-diff, which would be too slow. It assumes elements of different types produce different trees (unmount/remount rather than patch), and uses keys to match items within a list. The result is a minimal list of real DOM mutations, applied together in a single commit.

### Q: What is Fiber, and why was it introduced?
**Answer:** Fiber is React's internal reconciliation engine, rewritten in React 16. It represents each component/element as a "fiber" node in a tree that can be processed incrementally. Unlike the old stack-based reconciler — which had to finish a full re-render synchronously once started — Fiber can pause work, prioritize urgent updates, and resume later, which is what makes concurrent rendering and time-slicing possible.

### Q: What are the phases of a React render, and what happens in each?
**Answer:** The **render phase** builds the new tree and diffs it — this work is interruptible and shouldn't have visible side effects. The **commit phase** actually applies the calculated DOM mutations and runs the lifecycle methods/effects tied to that update (`useLayoutEffect` synchronously, `useEffect` asynchronously after paint) — this phase is synchronous and can't be interrupted.

### Q: What is Server-Side Rendering (SSR)?
**Answer:** SSR renders a page's initial HTML on the server using the same React component tree, and sends fully-formed HTML to the browser instead of an empty `<div id="root">` that JavaScript fills in later. This improves perceived load time and SEO, since content is visible and crawlable before JavaScript even downloads.

### Q: What is Static Site Generation (SSG), and how does it differ from SSR?
**Answer:** SSG renders pages to HTML once, at build time, and serves the same static file to every request — extremely fast and cacheable via a CDN, suited to content that doesn't change per request (blogs, docs, marketing pages). SSR renders on each request instead, so it can include per-request data (like a logged-in user's dashboard) but is comparatively slower since rendering happens live.

### Q: What is hydration?
**Answer:** Hydration is how React "attaches" to server-rendered HTML on the client — reusing the existing DOM nodes and wiring up event listeners and internal state, rather than throwing away the markup and rendering from scratch. For it to work correctly, the client's initial render output must match the server's HTML exactly, or React warns about a hydration mismatch.

### Q: What are Error Boundaries, and how do you implement one?
**Answer:** Error Boundaries are components that catch JavaScript errors thrown anywhere in their child tree during rendering, in lifecycle methods, and in constructors — logging the error and showing a fallback UI instead of crashing the whole app. They currently must be class components (`static getDerivedStateFromError` and/or `componentDidCatch`) — there's no Hook equivalent — and they don't catch errors in event handlers, async code, or during SSR.

**Example:**
```jsx
class ErrorBoundary extends React.Component {
  state = { hasError: false };
  static getDerivedStateFromError() { return { hasError: true }; }
  componentDidCatch(error, info) { logErrorToService(error, info); }
  render() {
    if (this.state.hasError) return <h1>Something went wrong.</h1>;
    return this.props.children;
  }
}
```

### Q: Why does changing a Context value re-render every consumer, even ones using only part of it?
**Answer:** `useContext` subscribes a component to the *entire* value — React doesn't inspect which specific property a component reads, it just re-renders any consumer whenever the Provider's `value` prop changes by reference. This is why it's common to split a large context into smaller, more focused contexts, or pair Context with a state library for more selective updates.

### Q: What's the difference between React elements, component instances, and DOM nodes?
**Answer:** A React element is a plain, immutable description of what to render — a lightweight blueprint. A component instance is the actual stateful realization of a class component that React keeps in memory between renders (function components don't have a persistent "instance" in the same sense — React tracks their Hook state separately via Fiber). A DOM node is the real browser object that finally appears on the page.

### Q: What is tree shaking, and how does it help a React app's bundle size?
**Answer:** Tree shaking is a build-time optimization (used by bundlers like Webpack, Rollup, or esbuild) that removes unused exports from the final bundle by statically analyzing ES module imports/exports. Because it relies on that static structure, importing an entire library (`import * as _ from 'lodash'`) can prevent effective tree shaking compared to importing just what you need (`import debounce from 'lodash/debounce'`).

### Q: What's the practical difference between legacy (synchronous) mode and concurrent mode?
**Answer:** In legacy mode, once React starts rendering an update, it must finish and commit before handling anything else — potentially blocking the main thread on large updates. In concurrent mode (enabled via `createRoot`), React can interrupt an in-progress low-priority render to handle something more urgent, like a keystroke, then resume or restart the lower-priority render afterward — making the app feel more responsive under load.

---

<a id="common-coding-challenges"></a>
## Common Coding Challenges

### Q: Build a custom useDebounce hook.
**Answer:** Delay updating a "debounced" copy of a value until the input stops changing for a set delay, cancelling the pending timer whenever the value changes again first.

**Example:**
```jsx
function useDebounce(value, delay = 300) {
  const [debouncedValue, setDebouncedValue] = useState(value);

  useEffect(() => {
    const timer = setTimeout(() => setDebouncedValue(value), delay);
    return () => clearTimeout(timer);
  }, [value, delay]);

  return debouncedValue;
}

// Usage: const debouncedSearch = useDebounce(searchTerm, 500);
```

### Q: Build a custom useToggle hook.
**Answer:** Wrap a boolean piece of state with a memoized function that flips it, so consumers get a clean, reusable on/off toggle.

**Example:**
```jsx
function useToggle(initialValue = false) {
  const [value, setValue] = useState(initialValue);
  const toggle = useCallback(() => setValue(v => !v), []);
  return [value, toggle];
}

// Usage: const [isOpen, toggleOpen] = useToggle();
```

### Q: Build a counter component with increment, decrement, and reset.
**Answer:** Classic useState exercise — three handlers updating one number, using the functional updater form for the increment/decrement to avoid stale-state bugs.

**Example:**
```jsx
function Counter() {
  const [count, setCount] = useState(0);
  return (
    <div>
      <p>{count}</p>
      <button onClick={() => setCount(c => c + 1)}>+</button>
      <button onClick={() => setCount(c => c - 1)}>-</button>
      <button onClick={() => setCount(0)}>Reset</button>
    </div>
  );
}
```

### Q: Build a simple Todo app (add, toggle, remove).
**Answer:** Store todos as an array of objects in state, and always update it immutably — spreading to add, mapping to toggle, filtering to remove.

**Example:**
```jsx
function TodoApp() {
  const [todos, setTodos] = useState([]);
  const [text, setText] = useState('');

  const addTodo = () => {
    if (!text.trim()) return;
    setTodos(prev => [...prev, { id: Date.now(), text, done: false }]);
    setText('');
  };
  const toggleTodo = id =>
    setTodos(prev => prev.map(t => (t.id === id ? { ...t, done: !t.done } : t)));
  const removeTodo = id =>
    setTodos(prev => prev.filter(t => t.id !== id));

  return (
    <div>
      <input value={text} onChange={e => setText(e.target.value)} />
      <button onClick={addTodo}>Add</button>
      <ul>
        {todos.map(t => (
          <li key={t.id} style={{ textDecoration: t.done ? 'line-through' : 'none' }}>
            <span onClick={() => toggleTodo(t.id)}>{t.text}</span>
            <button onClick={() => removeTodo(t.id)}>x</button>
          </li>
        ))}
      </ul>
    </div>
  );
}
```

### Q: Implement infinite scroll.
**Answer:** Watch a sentinel element at the bottom of the list with an `IntersectionObserver`, and load more items whenever it scrolls into view.

**Example:**
```jsx
function InfiniteList() {
  const [items, setItems] = useState(() => Array.from({ length: 20 }, (_, i) => i));
  const loaderRef = useRef(null);

  useEffect(() => {
    const observer = new IntersectionObserver(entries => {
      if (entries[0].isIntersecting) {
        setItems(prev => [...prev, ...Array.from({ length: 20 }, (_, i) => prev.length + i)]);
      }
    });
    if (loaderRef.current) observer.observe(loaderRef.current);
    return () => observer.disconnect();
  }, []);

  return (
    <div>
      {items.map(i => <div key={i}>Item {i}</div>)}
      <div ref={loaderRef}>Loading more...</div>
    </div>
  );
}
```

### Q: Implement a debounced search box component.
**Answer:** Combine a plain controlled input with the `useDebounce` hook above, and only fire the actual search call once the debounced value settles.

**Example:**
```jsx
function SearchBox({ onSearch }) {
  const [query, setQuery] = useState('');
  const debouncedQuery = useDebounce(query, 400);

  useEffect(() => {
    if (debouncedQuery) onSearch(debouncedQuery);
  }, [debouncedQuery, onSearch]);

  return <input value={query} onChange={e => setQuery(e.target.value)} placeholder="Search..." />;
}
```

### Q: Build a custom useFetch hook.
**Answer:** Encapsulate the loading/data/error state trio around a `fetch` call, guarding against setting state after the component unmounts.

**Example:**
```jsx
function useFetch(url) {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    let isMounted = true;
    setLoading(true);
    fetch(url)
      .then(res => res.json())
      .then(json => { if (isMounted) { setData(json); setLoading(false); } })
      .catch(err => { if (isMounted) { setError(err); setLoading(false); } });
    return () => { isMounted = false; };
  }, [url]);

  return { data, loading, error };
}
```

### Q: Build a custom usePrevious hook.
**Answer:** Use a ref that's updated in an effect (which runs *after* the render commits), so on any given render it still holds the value from the render before.

**Example:**
```jsx
function usePrevious(value) {
  const ref = useRef();
  useEffect(() => {
    ref.current = value;
  }, [value]);
  return ref.current; // value from before this render's update
}

// Usage: const prevCount = usePrevious(count);
```

### Q: Build a simple, accessible modal component.
**Answer:** Render nothing when closed, stop click events on the modal box from bubbling up to the overlay (so clicking inside doesn't close it), and close on overlay click or an explicit close button.

**Example:**
```jsx
function Modal({ isOpen, onClose, children }) {
  if (!isOpen) return null;
  return (
    <div className="overlay" onClick={onClose}>
      <div className="modal" onClick={e => e.stopPropagation()}>
        <button onClick={onClose}>×</button>
        {children}
      </div>
    </div>
  );
}
```

### Q: Build an accordion component.
**Answer:** Track which single index is open (or null), and toggle it closed if the same item is clicked again.

**Example:**
```jsx
function Accordion({ items }) {
  const [openIndex, setOpenIndex] = useState(null);

  return (
    <div>
      {items.map((item, index) => (
        <div key={item.id}>
          <button onClick={() => setOpenIndex(openIndex === index ? null : index)}>
            {item.title}
          </button>
          {openIndex === index && <div>{item.content}</div>}
        </div>
      ))}
    </div>
  );
}
```

### Q: Implement pagination for a list.
**Answer:** Keep the current page in state, slice the full array to the current page's range, and derive the total page count from the array length and page size.

**Example:**
```jsx
function PaginatedList({ items, pageSize = 10 }) {
  const [page, setPage] = useState(1);
  const totalPages = Math.ceil(items.length / pageSize);
  const currentItems = items.slice((page - 1) * pageSize, page * pageSize);

  return (
    <div>
      <ul>{currentItems.map(item => <li key={item.id}>{item.name}</li>)}</ul>
      <button disabled={page === 1} onClick={() => setPage(p => p - 1)}>Prev</button>
      <span> Page {page} of {totalPages} </span>
      <button disabled={page === totalPages} onClick={() => setPage(p => p + 1)}>Next</button>
    </div>
  );
}
```

### Q: Build a custom useLocalStorage hook.
**Answer:** Seed state from `localStorage` on first render (wrapped in a try/catch for safety), and sync back to `localStorage` in an effect whenever the value changes.

**Example:**
```jsx
function useLocalStorage(key, initialValue) {
  const [value, setValue] = useState(() => {
    try {
      const stored = window.localStorage.getItem(key);
      return stored ? JSON.parse(stored) : initialValue;
    } catch {
      return initialValue;
    }
  });

  useEffect(() => {
    window.localStorage.setItem(key, JSON.stringify(value));
  }, [key, value]);

  return [value, setValue];
}
```

---

<a id="behavioral-scenario-questions"></a>
## Behavioral / Scenario-Based Questions

### Q: How would you optimize a component rendering a list of 10,000 items?
**Answer:** Virtualize the list (`react-window`/`react-virtualized`) so only visible rows exist in the DOM, memoize row components with `React.memo` to skip re-rendering unaffected rows, make sure keys are stable, and move expensive per-item computation into `useMemo`. If the data supports it, consider pagination or infinite scroll instead of rendering everything at once.

### Q: How would you debug an infinite re-render loop?
**Answer:** Look for a `setState` call running unconditionally during render (not inside an event handler or effect), or a `useEffect` whose dependency array includes a value — an object, array, or function — that gets recreated every render, causing the effect to re-run and set state again indefinitely. React DevTools plus a few well-placed logs in the render body and effects usually pinpoint it quickly.

### Q: How would you structure a large-scale React application's folders?
**Answer:** A common approach is organizing "by feature/domain" — e.g., `features/auth`, `features/dashboard`, each bundling its own components, hooks, and state — rather than "by type" (all components in one folder, all hooks in another), which scales better as the app grows. Shared, reusable pieces (UI primitives, utilities, hooks) typically live in a common/shared directory.

### Q: How would you implement centralized error handling in a React app?
**Answer:** Wrap the app (or key sections) in Error Boundaries to catch render-time errors and show a fallback UI; centralize API error handling (e.g., an Axios interceptor or a wrapper around `fetch`) to catch network/HTTP errors consistently; and integrate an error-reporting service like Sentry to capture and alert on production errors.

### Q: How would you decide between Context API and Redux/Zustand for a new project?
**Answer:** Weigh the scale and update frequency of shared state, team familiarity, and whether you need dev tools like time-travel debugging or middleware. For a small app or infrequently-changing global values (theme, auth), Context is enough. For complex, frequently-updated state shared across many features, a dedicated library gives better performance and tooling out of the box.

### Q: How would you implement authentication with protected routes?
**Answer:** Store auth state (a token, user info) in Context or a state library, persist it thoughtfully (in-memory plus an httpOnly refresh-token cookie is safer than `localStorage` alone, given XSS risk), and wrap protected routes in a component that checks this state and redirects unauthenticated users to a login page.

### Q: How would you approach migrating a legacy class-component codebase to hooks?
**Answer:** Migrate incrementally — hooks and class components can coexist in the same app, so there's no need for a disruptive rewrite. Start with leaf/simple components, extract shared lifecycle logic into custom hooks as you go, and prioritize components you're already touching for other reasons.

### Q: How would you fix "Can't perform a React state update on an unmounted component"?
**Answer:** This happens when an async operation (like a fetch) resolves after the component has already unmounted, and its callback still tries to call a state setter. Fix it by tracking whether the component is still mounted (a ref-based flag) before calling setState, or by cancelling the request in the effect's cleanup with an `AbortController`.

### Q: How would you implement dark mode / theming in a React app?
**Answer:** Store the current theme in Context (or a small state library) near the top of the app, apply it via a CSS class or data attribute on the root element (or CSS variables components reference), and persist the user's preference in `localStorage` — often defaulting to the OS-level `prefers-color-scheme` media query.

### Q: What would you look for when reviewing a teammate's React pull request?
**Answer:** Correctness and edge cases (loading/error/empty states); proper key usage in lists; unnecessary re-renders or missing memoization where it actually matters; correct and complete `useEffect` dependency arrays; accessibility (semantic HTML, labels, keyboard navigation); and whether logic could be simplified or extracted into a reusable hook or component.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to architecture.
- **Revising the night before?** Jump straight to [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions), then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
