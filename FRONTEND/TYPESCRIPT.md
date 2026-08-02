# TypeScript Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of TypeScript interview questions — from core types and interfaces to generics, advanced/utility types, classes, decorators, and tooling — with clear answers and code examples where they help. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#-most-asked--tricky-questions)
  - [What is TypeScript, and how does it relate to JavaScript?](#what-is-typescript-and-how-does-it-relate-to-javascript)
  - [What is the difference between `interface` and `type` in TypeScript?](#what-is-the-difference-between-interface-and-type-in-typescript)
  - [What is the difference between `any` and `unknown`?](#what-is-the-difference-between-any-and-unknown)
  - [What is type narrowing?](#what-is-type-narrowing)
  - [What is a generic in TypeScript, and why is it useful?](#what-is-a-generic-in-typescript-and-why-is-it-useful)
  - [What is the difference between `interface` extension and `type` intersection?](#what-is-the-difference-between-interface-extension-and-type-intersection)
  - [What is structural typing, and how does it differ from nominal typing?](#what-is-structural-typing-and-how-does-it-differ-from-nominal-typing)
  - [What is the difference between `readonly` and `const`?](#what-is-the-difference-between-readonly-and-const)
  - [What are type guards, and how do you write a custom one?](#what-are-type-guards-and-how-do-you-write-a-custom-one)
  - [What is the difference between `never` and `void`?](#what-is-the-difference-between-never-and-void)
  - [What does the `keyof` operator do?](#what-does-the-keyof-operator-do)
  - [What is a discriminated union, and why is it useful?](#what-is-a-discriminated-union-and-why-is-it-useful)
  - [What is the difference between a type assertion (`as`) and type casting in languages like Java or C#?](#what-is-the-difference-between-a-type-assertion-as-and-type-casting-in-languages-like-java-or-c)
  - [What does the `satisfies` operator do, and what problem does it solve?](#what-does-the-satisfies-operator-do-and-what-problem-does-it-solve)
  - [What is the difference between compile-time type checking and runtime behavior in TypeScript?](#what-is-the-difference-between-compile-time-type-checking-and-runtime-behavior-in-typescript)
- [TypeScript Basics](#typescript-basics)
  - [How do you install and compile a TypeScript file?](#how-do-you-install-and-compile-a-typescript-file)
  - [What is type inference, and why does it reduce the need for explicit annotations?](#what-is-type-inference-and-why-does-it-reduce-the-need-for-explicit-annotations)
  - [What are the basic primitive types in TypeScript?](#what-are-the-basic-primitive-types-in-typescript)
  - [How do you type an array, and what are the two equivalent syntaxes?](#how-do-you-type-an-array-and-what-are-the-two-equivalent-syntaxes)
  - [What is a tuple, and how does it differ from a regular array?](#what-is-a-tuple-and-how-does-it-differ-from-a-regular-array)
  - [What does the `strict` compiler flag actually enable?](#what-does-the-strict-compiler-flag-actually-enable)
  - [What is `strictNullChecks`, and what does it change?](#what-is-strictnullchecks-and-what-does-it-change)
  - [What is the difference between `undefined` and an optional property (`prop?: type`)?](#what-is-the-difference-between-undefined-and-an-optional-property-prop-type)
  - [What is the difference between a `.ts` file and a `.tsx` file?](#what-is-the-difference-between-a-ts-file-and-a-tsx-file)
  - [What is a declaration file (`.d.ts`), and what is it used for?](#what-is-a-declaration-file-dts-and-what-is-it-used-for)
- [Types & Type Annotations](#types--type-annotations)
  - [What is the difference between a type annotation and a type assertion?](#what-is-the-difference-between-a-type-annotation-and-a-type-assertion)
  - [What is a literal type?](#what-is-a-literal-type)
  - [What is a union type, and how do you declare one?](#what-is-a-union-type-and-how-do-you-declare-one)
  - [What is an intersection type, and how do you declare one?](#what-is-an-intersection-type-and-how-do-you-declare-one)
  - [What is the difference between `string[]` and `Array<string>`?](#what-is-the-difference-between-string-and-arraystring)
  - [What is type widening, and when does it happen?](#what-is-type-widening-and-when-does-it-happen)
  - [What is the `const` assertion (`as const`), and what does it do?](#what-is-the-const-assertion-as-const-and-what-does-it-do)
  - [What is the difference between a nullable type and an optional parameter?](#what-is-the-difference-between-a-nullable-type-and-an-optional-parameter)
  - [What is a template literal type?](#what-is-a-template-literal-type)
  - [What is the difference between `object`, `Object`, and `{}` as types?](#what-is-the-difference-between-object-object-and--as-types)
- [Interfaces vs Type Aliases](#interfaces-vs-type-aliases)
  - [How do you extend one interface with another?](#how-do-you-extend-one-interface-with-another)
  - [What is declaration merging, and which of `interface`/`type` supports it?](#what-is-declaration-merging-and-which-of-interfacetype-supports-it)
  - [How would you make all properties on an interface optional without rewriting each one?](#how-would-you-make-all-properties-on-an-interface-optional-without-rewriting-each-one)
  - [Can a `type` alias represent a union or a primitive, and can an `interface`?](#can-a-type-alias-represent-a-union-or-a-primitive-and-can-an-interface)
  - [How do you make a class implement an interface, and what does that guarantee?](#how-do-you-make-a-class-implement-an-interface-and-what-does-that-guarantee)
  - [What are index signatures, and when would you use one on an interface?](#what-are-index-signatures-and-when-would-you-use-one-on-an-interface)
  - [What are optional and readonly properties on an interface?](#what-are-optional-and-readonly-properties-on-an-interface)
  - [When would you generally prefer `type` over `interface`, and vice versa?](#when-would-you-generally-prefer-type-over-interface-and-vice-versa)
- [Functions](#functions)
  - [How do you type a function's parameters and return value?](#how-do-you-type-a-functions-parameters-and-return-value)
  - [What is an optional parameter, and where must it appear in the parameter list?](#what-is-an-optional-parameter-and-where-must-it-appear-in-the-parameter-list)
  - [What is a default parameter, and how does it interact with the parameter's type?](#what-is-a-default-parameter-and-how-does-it-interact-with-the-parameters-type)
  - [How do you type rest parameters?](#how-do-you-type-rest-parameters)
  - [What is a function overload in TypeScript?](#what-is-a-function-overload-in-typescript)
  - [What is the difference between typing a function with an arrow function type vs. a call signature in an interface?](#what-is-the-difference-between-typing-a-function-with-an-arrow-function-type-vs-a-call-signature-in-an-interface)
  - [How does TypeScript type `this` inside a function, and what is a `this` parameter?](#how-does-typescript-type-this-inside-a-function-and-what-is-a-this-parameter)
  - [What is a generic function constraint, and how do you write one?](#what-is-a-generic-function-constraint-and-how-do-you-write-one)
- [Classes & OOP](#classes--oop)
  - [What are the access modifiers in TypeScript classes, and what does each restrict?](#what-are-the-access-modifiers-in-typescript-classes-and-what-does-each-restrict)
  - [What is the difference between TypeScript's `private` keyword and JavaScript's native `#` private fields?](#what-is-the-difference-between-typescripts-private-keyword-and-javascripts-native--private-fields)
  - [What is a parameter property in a TypeScript class constructor?](#what-is-a-parameter-property-in-a-typescript-class-constructor)
  - [What does the `abstract` keyword do on a class or method?](#what-does-the-abstract-keyword-do-on-a-class-or-method)
  - [How does TypeScript type static properties and methods, and how are they accessed?](#how-does-typescript-type-static-properties-and-methods-and-how-are-they-accessed)
  - [How does generics apply to classes in TypeScript?](#how-does-generics-apply-to-classes-in-typescript)
  - [What is method overriding in a TypeScript subclass, and what does the `override` keyword add?](#what-is-method-overriding-in-a-typescript-subclass-and-what-does-the-override-keyword-add)
  - [What is the difference between an interface and an abstract class for defining a contract?](#what-is-the-difference-between-an-interface-and-an-abstract-class-for-defining-a-contract)
  - [What are getters and setters in a TypeScript class, and how are they typed?](#what-are-getters-and-setters-in-a-typescript-class-and-how-are-they-typed)
  - [What does implementing multiple interfaces on a single class look like, and does TypeScript support multiple inheritance of classes?](#what-does-implementing-multiple-interfaces-on-a-single-class-look-like-and-does-typescript-support-multiple-inheritance-of-classes)
- [Generics](#generics)
  - [What problem do generics solve that `any` doesn't?](#what-problem-do-generics-solve-that-any-doesnt)
  - [How does TypeScript infer generic type arguments, and when do you need to specify them explicitly?](#how-does-typescript-infer-generic-type-arguments-and-when-do-you-need-to-specify-them-explicitly)
  - [What is a generic constraint, and how do you write one with `extends`?](#what-is-a-generic-constraint-and-how-do-you-write-one-with-extends)
  - [What are default generic type parameters?](#what-are-default-generic-type-parameters)
  - [How would you write a generic function that works on any array and returns its first element?](#how-would-you-write-a-generic-function-that-works-on-any-array-and-returns-its-first-element)
  - [What is the difference between a generic type parameter used on a function versus one used on the whole class/interface?](#what-is-the-difference-between-a-generic-type-parameter-used-on-a-function-versus-one-used-on-the-whole-classinterface)
  - [What is `keyof T` combined with a generic used for, e.g. in a generic "get property" function?](#what-is-keyof-t-combined-with-a-generic-used-for-eg-in-a-generic-get-property-function)
  - [What are variance and generic type parameter positions (roughly), and why does it sometimes matter for function types?](#what-are-variance-and-generic-type-parameter-positions-roughly-and-why-does-it-sometimes-matter-for-function-types)
  - [How do generics interact with default values/inference when using React-style generic components or hooks?](#how-do-generics-interact-with-default-valuesinference-when-using-react-style-generic-components-or-hooks)
  - [What is a conditional type used together with generics for, at a basic level?](#what-is-a-conditional-type-used-together-with-generics-for-at-a-basic-level)
- [Union, Intersection & Literal Types](#union-intersection--literal-types)
  - [How do you narrow a union type using `typeof`?](#how-do-you-narrow-a-union-type-using-typeof)
  - [How do you narrow a union of object types using a shared discriminant property?](#how-do-you-narrow-a-union-of-object-types-using-a-shared-discriminant-property)
  - [What happens when you access a property that only exists on some members of a union type, without narrowing first?](#what-happens-when-you-access-a-property-that-only-exists-on-some-members-of-a-union-type-without-narrowing-first)
  - [What is the difference between a union type and an enum for representing a fixed set of options?](#what-is-the-difference-between-a-union-type-and-an-enum-for-representing-a-fixed-set-of-options)
  - [How do intersection types behave when combining two object types with a property of the same name but incompatible types?](#how-do-intersection-types-behave-when-combining-two-object-types-with-a-property-of-the-same-name-but-incompatible-types)
  - [What is a nullable union type, and how do you safely work with one under `strictNullChecks`?](#what-is-a-nullable-union-type-and-how-do-you-safely-work-with-one-under-strictnullchecks)
  - [Can you use a union type as a function parameter, and what are the implications for the function body?](#can-you-use-a-union-type-as-a-function-parameter-and-what-are-the-implications-for-the-function-body)
  - [What is an exhaustiveness check using `never`, and why is it useful with discriminated unions?](#what-is-an-exhaustiveness-check-using-never-and-why-is-it-useful-with-discriminated-unions)
- [Advanced & Utility Types](#advanced--utility-types)
  - [What does `Partial<T>` do?](#what-does-partialt-do)
  - [What does `Pick<T, K>` and `Omit<T, K>` do?](#what-does-pickt-k-and-omitt-k-do)
  - [What does `Record<K, V>` do, and when is it useful?](#what-does-recordk-v-do-and-when-is-it-useful)
  - [What does `ReturnType<T>` do, and what is a common use case?](#what-does-returntypet-do-and-what-is-a-common-use-case)
  - [What is a mapped type, and how would you write a simplified version of `Readonly<T>` yourself?](#what-is-a-mapped-type-and-how-would-you-write-a-simplified-version-of-readonlyt-yourself)
  - [What is a conditional type, and how does `infer` work within one?](#what-is-a-conditional-type-and-how-does-infer-work-within-one)
  - [What does `Required<T>` do, and how does it differ from `Partial<T>`?](#what-does-requiredt-do-and-how-does-it-differ-from-partialt)
  - [What is a distributive conditional type?](#what-is-a-distributive-conditional-type)
  - [What does `Exclude<T, U>` and `Extract<T, U>` do?](#what-does-excludet-u-and-extractt-u-do)
  - [What is the difference between `Awaited<T>` and just accessing the resolved type of a `Promise` manually?](#what-is-the-difference-between-awaitedt-and-just-accessing-the-resolved-type-of-a-promise-manually)
- [Type Narrowing & Guards](#type-narrowing--guards)
  - [What is the `in` operator used for as a type guard?](#what-is-the-in-operator-used-for-as-a-type-guard)
  - [What is the `instanceof` operator used for as a type guard, and what kind of types does it work with?](#what-is-the-instanceof-operator-used-for-as-a-type-guard-and-what-kind-of-types-does-it-work-with)
  - [How does TypeScript narrow a type based on a truthy check, e.g. `if (value)`?](#how-does-typescript-narrow-a-type-based-on-a-truthy-check-eg-if-value)
  - [What is a user-defined type predicate function, and what makes its signature special?](#what-is-a-user-defined-type-predicate-function-and-what-makes-its-signature-special)
  - [How does TypeScript narrow within an `else` branch, or after an early `return`?](#how-does-typescript-narrow-within-an-else-branch-or-after-an-early-return)
  - [What is the difference between narrowing with `==`/`!=` versus `===`/`!==` against `null`?](#what-is-the-difference-between-narrowing-with--versus--against-null)
  - [Can you narrow a type using a value stored in a variable rather than an inline condition, e.g. assigning `const isString = typeof x === "string"` first?](#can-you-narrow-a-type-using-a-value-stored-in-a-variable-rather-than-an-inline-condition-eg-assigning-const-isstring--typeof-x--string-first)
  - [What is assertion-based narrowing with `asserts` functions, and how does it differ from a type predicate function?](#what-is-assertion-based-narrowing-with-asserts-functions-and-how-does-it-differ-from-a-type-predicate-function)
- [Enums](#enums)
  - [What is an enum in TypeScript, and what does it compile down to by default?](#what-is-an-enum-in-typescript-and-what-does-it-compile-down-to-by-default)
  - [What is the difference between a numeric enum and a string enum?](#what-is-the-difference-between-a-numeric-enum-and-a-string-enum)
  - [What is a `const enum`, and how does it differ from a regular enum at compile time?](#what-is-a-const-enum-and-how-does-it-differ-from-a-regular-enum-at-compile-time)
  - [What are some common criticisms of enums, and what alternative do many teams prefer?](#what-are-some-common-criticisms-of-enums-and-what-alternative-do-many-teams-prefer)
  - [Can you assign a plain number directly to a numeric enum-typed variable?](#can-you-assign-a-plain-number-directly-to-a-numeric-enum-typed-variable)
  - [How would you iterate over the members of a string enum?](#how-would-you-iterate-over-the-members-of-a-string-enum)
- [Modules & Namespaces](#modules--namespaces)
  - [What is the difference between an ES module and a TypeScript namespace?](#what-is-the-difference-between-an-es-module-and-a-typescript-namespace)
  - [What is the difference between a default export and a named export in TypeScript?](#what-is-the-difference-between-a-default-export-and-a-named-export-in-typescript)
  - [What does `export type` (a type-only export) do, and why would you use it?](#what-does-export-type-a-type-only-export-do-and-why-would-you-use-it)
  - [What is module augmentation, and what is it used for?](#what-is-module-augmentation-and-what-is-it-used-for)
  - [What is the difference between `import type` and a regular `import`?](#what-is-the-difference-between-import-type-and-a-regular-import)
  - [What is a barrel file, and what's a potential downside of using one?](#what-is-a-barrel-file-and-whats-a-potential-downside-of-using-one)
- [Decorators](#decorators)
  - [What is a decorator in TypeScript, and what does it let you do?](#what-is-a-decorator-in-typescript-and-what-does-it-let-you-do)
  - [What is the difference between a class decorator and a method decorator?](#what-is-the-difference-between-a-class-decorator-and-a-method-decorator)
  - [How do you enable decorators in a TypeScript project, and why aren't they on by default?](#how-do-you-enable-decorators-in-a-typescript-project-and-why-arent-they-on-by-default)
  - [What is a decorator factory?](#what-is-a-decorator-factory)
  - [What is `reflect-metadata`, and how does it relate to decorators in frameworks like NestJS?](#what-is-reflect-metadata-and-how-does-it-relate-to-decorators-in-frameworks-like-nestjs)
  - [What order do multiple decorators applied to the same declaration run in?](#what-order-do-multiple-decorators-applied-to-the-same-declaration-run-in)
- [tsconfig & Tooling](#tsconfig--tooling)
  - [What is `tsconfig.json`, and what is its basic purpose?](#what-is-tsconfigjson-and-what-is-its-basic-purpose)
  - [What does the `target` compiler option control?](#what-does-the-target-compiler-option-control)
  - [What does the `module` compiler option control?](#what-does-the-module-compiler-option-control)
  - [What is the difference between `noImplicitAny` and `strict`?](#what-is-the-difference-between-noimplicitany-and-strict)
  - [What does `esModuleInterop` do, and what problem does it solve?](#what-does-esmoduleinterop-do-and-what-problem-does-it-solve)
  - [What is the difference between `tsc --noEmit` and a regular `tsc` build?](#what-is-the-difference-between-tsc---noemit-and-a-regular-tsc-build)
  - [What does the `skipLibCheck` option do, and why might a project enable it?](#what-does-the-skiplibcheck-option-do-and-why-might-a-project-enable-it)
  - [What is the difference between using `tsc` directly versus a tool like Babel, esbuild, or SWC to compile TypeScript?](#what-is-the-difference-between-using-tsc-directly-versus-a-tool-like-babel-esbuild-or-swc-to-compile-typescript)
- [Behavioral / Scenario-Based Questions](#behavioral--scenario-based-questions)
  - [You're converting a large existing JavaScript codebase to TypeScript — how would you approach it?](#youre-converting-a-large-existing-javascript-codebase-to-typescript--how-would-you-approach-it)
  - [A third-party JavaScript library you depend on has no official TypeScript types — how would you handle it?](#a-third-party-javascript-library-you-depend-on-has-no-official-typescript-types--how-would-you-handle-it)
  - [A colleague keeps using `any` to quickly silence type errors instead of fixing them properly — how would you address this in a code review?](#a-colleague-keeps-using-any-to-quickly-silence-type-errors-instead-of-fixing-them-properly--how-would-you-address-this-in-a-code-review)
  - [You're seeing a confusing TypeScript error about incompatible types that doesn't clearly explain the actual problem — how would you debug it?](#youre-seeing-a-confusing-typescript-error-about-incompatible-types-that-doesnt-clearly-explain-the-actual-problem--how-would-you-debug-it)
  - [How would you decide whether to model a piece of state as a union of string literals versus an enum?](#how-would-you-decide-whether-to-model-a-piece-of-state-as-a-union-of-string-literals-versus-an-enum)
  - [How would you type an API response where the shape isn't fully guaranteed to match your TypeScript types at runtime?](#how-would-you-type-an-api-response-where-the-shape-isnt-fully-guaranteed-to-match-your-typescript-types-at-runtime)
  - [How would you approach reviewing a pull request that introduces a lot of new generic types you find hard to follow?](#how-would-you-approach-reviewing-a-pull-request-that-introduces-a-lot-of-new-generic-types-you-find-hard-to-follow)
  - [A generic utility function you wrote type-checks fine but produces confusing autocomplete/hover types for consumers — how would you improve it?](#a-generic-utility-function-you-wrote-type-checks-fine-but-produces-confusing-autocompletehover-types-for-consumers--how-would-you-improve-it)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="-most-asked--tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every TypeScript interview. If you're short on time, start here.

<a id="what-is-typescript-and-how-does-it-relate-to-javascript"></a>
### Q: What is TypeScript, and how does it relate to JavaScript?
**Answer:** TypeScript is a statically-typed superset of JavaScript that compiles down to plain JavaScript. Every valid JavaScript program is (almost) valid TypeScript, and TypeScript adds optional static type checking, interfaces, generics, and other tooling on top, purely at compile time — none of it exists at runtime.

<a id="what-is-the-difference-between-interface-and-type-in-typescript"></a>
### Q: What is the difference between `interface` and `type` in TypeScript?
**Answer:** Both can describe the shape of an object, and in many cases are interchangeable. Key differences: `interface` supports declaration merging (multiple declarations with the same name automatically combine) and is generally preferred for public object/class APIs; `type` can describe unions, intersections, tuples, and primitives directly, which `interface` cannot express on its own.

<a id="what-is-the-difference-between-any-and-unknown"></a>
### Q: What is the difference between `any` and `unknown`?
**Answer:** `any` opts a value entirely out of type checking — you can do anything with it with no compiler complaints, effectively disabling TypeScript's safety for that value. `unknown` is also a top type that can hold any value, but the compiler forces you to narrow its type (with a type guard or assertion) before you can perform most operations on it, making it a much safer alternative.

<a id="what-is-type-narrowing"></a>
### Q: What is type narrowing?
**Answer:** The process by which TypeScript automatically refines a variable's broader type to a more specific one within a certain block of code, based on control-flow checks like `typeof`, `instanceof`, truthy checks, or custom type guards — letting you safely access properties/methods specific to the narrowed type.

<a id="what-is-a-generic-in-typescript-and-why-is-it-useful"></a>
### Q: What is a generic in TypeScript, and why is it useful?
**Answer:** A generic lets you write a function, class, or type that works with a range of types rather than a single one, while still preserving type information — the specific type is supplied (or inferred) at the point of use, rather than the definition being hardcoded to one particular type.

**Example:**
```ts
function identity<T>(value: T): T {
  return value;
}
identity<string>("hello"); // T is string
```

<a id="what-is-the-difference-between-interface-extension-and-type-intersection"></a>
### Q: What is the difference between `interface` extension and `type` intersection?
**Answer:** An interface extends another with the `extends` keyword, and if the extending interface redeclares a property incompatibly, TypeScript raises an error immediately. A type intersection (`TypeA & TypeB`) combines two types structurally; if the two have conflicting property types, the resulting type for that property silently becomes `never` rather than raising an upfront error.

<a id="what-is-structural-typing-and-how-does-it-differ-from-nominal-typing"></a>
### Q: What is structural typing, and how does it differ from nominal typing?
**Answer:** TypeScript uses structural typing ("duck typing") — two types are considered compatible if they have the same shape, regardless of their declared names or where they were defined. Nominal typing (used by languages like Java or C#) instead considers two types compatible only if they're explicitly declared as related, even if their structure is identical.

<a id="what-is-the-difference-between-readonly-and-const"></a>
### Q: What is the difference between `readonly` and `const`?
**Answer:** `const` prevents reassigning a variable binding itself, but doesn't affect the mutability of an object it points to. `readonly` is applied to a property on an interface/type or class, preventing that specific property from being reassigned after initial assignment — it doesn't make the whole object immutable either, and both are compile-time-only checks with no runtime enforcement.

<a id="what-are-type-guards-and-how-do-you-write-a-custom-one"></a>
### Q: What are type guards, and how do you write a custom one?
**Answer:** A type guard is an expression that, when checked in a conditional, lets TypeScript narrow a variable's type within that branch. Built-in examples include `typeof`, `instanceof`, and `in`. A custom type guard is a function whose return type is a type predicate (`value is SomeType`), letting you encapsulate more complex narrowing logic.

**Example:**
```ts
function isString(value: unknown): value is string {
  return typeof value === "string";
}
```

<a id="what-is-the-difference-between-never-and-void"></a>
### Q: What is the difference between `never` and `void`?
**Answer:** `void` represents the absence of a meaningful return value — a function that doesn't explicitly return anything. `never` represents a value that can never actually occur at all — used for functions that always throw an error or contain an infinite loop, and never actually complete normally.

<a id="what-does-the-keyof-operator-do"></a>
### Q: What does the `keyof` operator do?
**Answer:** It produces a union of string (or number/symbol) literal types representing all the known property keys of a given type.

**Example:**
```ts
interface User { id: number; name: string; }
type UserKey = keyof User; // "id" | "name"
```

<a id="what-is-a-discriminated-union-and-why-is-it-useful"></a>
### Q: What is a discriminated union, and why is it useful?
**Answer:** A union of object types that share a common literal property (the "discriminant" or "tag"), letting TypeScript automatically narrow the exact type in a conditional just by checking that one property — extremely useful for safely modeling variant data like API responses or Redux-style actions.

**Example:**
```ts
type Shape =
  | { kind: "circle"; radius: number }
  | { kind: "square"; side: number };

function area(shape: Shape) {
  if (shape.kind === "circle") return Math.PI * shape.radius ** 2;
  return shape.side ** 2;
}
```

<a id="what-is-the-difference-between-a-type-assertion-as-and-type-casting-in-languages-like-java-or-c"></a>
### Q: What is the difference between a type assertion (`as`) and type casting in languages like Java or C#?
**Answer:** A TypeScript type assertion tells the compiler "trust me, treat this value as this type" purely at compile time — it performs no actual runtime conversion or validation, and an incorrect assertion can cause a runtime error later. A cast in languages like Java actually checks and converts the value at runtime, throwing immediately if it's invalid.

<a id="what-does-the-satisfies-operator-do-and-what-problem-does-it-solve"></a>
### Q: What does the `satisfies` operator do, and what problem does it solve?
**Answer:** `satisfies` checks that a value matches a given type without widening the value's own inferred type the way an explicit type annotation would — so you get validation against the type, while still keeping the most specific inferred type (e.g. a literal type) for later use, like autocompletion on a specific property.

**Example:**
```ts
const config = { mode: "dark" } satisfies { mode: "dark" | "light" };
// config.mode is still typed as "dark", not "dark" | "light"
```

<a id="what-is-the-difference-between-compile-time-type-checking-and-runtime-behavior-in-typescript"></a>
### Q: What is the difference between compile-time type checking and runtime behavior in TypeScript?
**Answer:** TypeScript's type system exists entirely at compile time — after compilation to JavaScript, all types are erased, and none of TypeScript's checks exist or run at runtime. This is why TypeScript can't catch things like malformed data arriving from an external API call at runtime; that still requires actual runtime validation (e.g. with a library like Zod), not just a type annotation.

---

<a id="typescript-basics"></a>
## TypeScript Basics

<a id="how-do-you-install-and-compile-a-typescript-file"></a>
### Q: How do you install and compile a TypeScript file?
**Answer:** Install the compiler with `npm install -g typescript` (or as a dev dependency), then compile a file with `tsc filename.ts`, which produces a corresponding `.js` file. Most projects instead run `tsc` against a `tsconfig.json` covering the whole project.

<a id="what-is-type-inference-and-why-does-it-reduce-the-need-for-explicit-annotations"></a>
### Q: What is type inference, and why does it reduce the need for explicit annotations?
**Answer:** TypeScript can automatically determine a variable's type from its initial value or usage context, without an explicit annotation — e.g. `let x = 5` is inferred as `number` — letting you write concise code while still getting full type safety, reserving explicit annotations for function parameters and cases the compiler can't infer on its own.

<a id="what-are-the-basic-primitive-types-in-typescript"></a>
### Q: What are the basic primitive types in TypeScript?
**Answer:** `string`, `number`, `boolean`, `null`, `undefined`, `bigint`, and `symbol` — mirroring JavaScript's own primitives, plus TypeScript-specific additions like `any`, `unknown`, `never`, and `void` for type-system purposes.

<a id="how-do-you-type-an-array-and-what-are-the-two-equivalent-syntaxes"></a>
### Q: How do you type an array, and what are the two equivalent syntaxes?
**Answer:** `number[]` or the generic form `Array<number>` — both are functionally identical; `T[]` is generally more common for simple element types, while `Array<T>` can read more clearly for complex generic types.

<a id="what-is-a-tuple-and-how-does-it-differ-from-a-regular-array"></a>
### Q: What is a tuple, and how does it differ from a regular array?
**Answer:** A tuple is a fixed-length array where each position has a specific, individually declared type, unlike a regular array where every element shares the same type.

**Example:**
```ts
let point: [number, number] = [10, 20];
```

<a id="what-does-the-strict-compiler-flag-actually-enable"></a>
### Q: What does the `strict` compiler flag actually enable?
**Answer:** It's a shorthand that turns on a whole bundle of stricter type-checking flags at once, including `strictNullChecks`, `noImplicitAny`, `strictFunctionTypes`, and several others — generally recommended for all new projects, since it catches significantly more potential bugs than TypeScript's default, looser configuration.

<a id="what-is-strictnullchecks-and-what-does-it-change"></a>
### Q: What is `strictNullChecks`, and what does it change?
**Answer:** With it enabled, `null` and `undefined` are only assignable to their own types (and `any`/`unknown`) rather than being valid values for every type by default — forcing you to explicitly handle the possibility of a value being missing wherever it's actually possible, rather than that being silently allowed everywhere.

<a id="what-is-the-difference-between-undefined-and-an-optional-property-prop-type"></a>
### Q: What is the difference between `undefined` and an optional property (`prop?: type`)?
**Answer:** An optional property (`age?: number`) can be entirely omitted from an object, in which case accessing it returns `undefined`, and its type is effectively `number | undefined`. Explicitly typing a property as `age: number | undefined` requires the property key to still be present on the object, just potentially holding the value `undefined`.

<a id="what-is-the-difference-between-a-ts-file-and-a-tsx-file"></a>
### Q: What is the difference between a `.ts` file and a `.tsx` file?
**Answer:** `.tsx` is used for TypeScript files that contain JSX syntax (typically React components) — the compiler needs this distinct extension to correctly parse the `<Tag>` syntax, which would otherwise be ambiguous with TypeScript's generic type-argument syntax `<T>`.

<a id="what-is-a-declaration-file-dts-and-what-is-it-used-for"></a>
### Q: What is a declaration file (`.d.ts`), and what is it used for?
**Answer:** A file containing only type information — no actual runtime code/implementation — used to describe the shape of existing JavaScript code (like a plain-JS library) so TypeScript can type-check code that uses it, without needing that library itself to be rewritten in TypeScript.

---

<a id="types--type-annotations"></a>
## Types & Type Annotations

<a id="what-is-the-difference-between-a-type-annotation-and-a-type-assertion"></a>
### Q: What is the difference between a type annotation and a type assertion?
**Answer:** A type annotation (`let x: number = 5`) declares a variable's type upfront, and the compiler verifies the assigned value actually matches it. A type assertion (`value as SomeType`) overrides the compiler's own inferred type for an existing value, without any actual verification that the assertion is correct.

<a id="what-is-a-literal-type"></a>
### Q: What is a literal type?
**Answer:** A type that represents one specific, exact value, rather than a whole category of values — e.g. the type `"success"` only accepts the exact string `"success"`, not any arbitrary string. Literal types are the building blocks of union types like `"success" | "error" | "loading"`.

<a id="what-is-a-union-type-and-how-do-you-declare-one"></a>
### Q: What is a union type, and how do you declare one?
**Answer:** A union type (`TypeA | TypeB`) means a value can be one of several specified types. You typically need to narrow a union with a type guard before accessing members specific to just one of its member types.

<a id="what-is-an-intersection-type-and-how-do-you-declare-one"></a>
### Q: What is an intersection type, and how do you declare one?
**Answer:** An intersection type (`TypeA & TypeB`) combines multiple types into one that must satisfy all of them simultaneously — an object of an intersection type must have every property required by each of the combined types.

<a id="what-is-the-difference-between-string-and-arraystring"></a>
### Q: What is the difference between `string[]` and `Array<string>`?
**Answer:** They're exactly equivalent — `string[]` is shorthand syntax, and `Array<string>` is the same type expressed using its generic form directly.

<a id="what-is-type-widening-and-when-does-it-happen"></a>
### Q: What is type widening, and when does it happen?
**Answer:** When TypeScript infers a broader, more general type than the literal value would suggest — e.g. `let x = "hello"` infers `x` as the general `string` type, not the literal type `"hello"`, since `let` variables are expected to be reassigned. Declaring with `const` instead usually infers the narrower literal type, since a `const` can never be reassigned.

<a id="what-is-the-const-assertion-as-const-and-what-does-it-do"></a>
### Q: What is the `const` assertion (`as const`), and what does it do?
**Answer:** It tells the compiler to infer the narrowest, most literal possible type for a value, and to treat array/object contents as `readonly`, rather than widening to general types like `string` or `number[]`.

**Example:**
```ts
const colors = ["red", "green"] as const;
// type is readonly ["red", "green"], not string[]
```

<a id="what-is-the-difference-between-a-nullable-type-and-an-optional-parameter"></a>
### Q: What is the difference between a nullable type and an optional parameter?
**Answer:** A nullable type (`string | null`) means the value must be explicitly present, but that presence can be the value `null`. An optional parameter (`name?: string`) means the argument can be omitted entirely when calling the function, in which case it's `undefined` inside the function body — the two express different absences and aren't automatically interchangeable.

<a id="what-is-a-template-literal-type"></a>
### Q: What is a template literal type?
**Answer:** A type built using JavaScript-style template literal syntax at the type level, combining literal string types (and other types) into new, more specific string literal types.

**Example:**
```ts
type Direction = "top" | "bottom";
type ClassName = `border-${Direction}`; // "border-top" | "border-bottom"
```

<a id="what-is-the-difference-between-object-object-and--as-types"></a>
### Q: What is the difference between `object`, `Object`, and `{}` as types?
**Answer:** `object` refers to any non-primitive value (excludes `string`, `number`, `boolean`, etc., but includes arrays, functions, and plain objects). `Object` (capitalized) refers to anything with the properties of JavaScript's base `Object` prototype, which is nearly everything including primitives, making it rarely useful. `{}` describes any value that isn't `null` or `undefined`, regardless of its actual shape — none of the three are the same as an actual empty object literal type in practice.

---

<a id="interfaces-vs-type-aliases"></a>
## Interfaces vs Type Aliases

<a id="how-do-you-extend-one-interface-with-another"></a>
### Q: How do you extend one interface with another?
**Answer:** Using the `extends` keyword — the extending interface inherits all members of the base interface and can add or (compatibly) narrow additional ones.

**Example:**
```ts
interface Animal { name: string; }
interface Dog extends Animal { breed: string; }
```

<a id="what-is-declaration-merging-and-which-of-interfacetype-supports-it"></a>
### Q: What is declaration merging, and which of `interface`/`type` supports it?
**Answer:** Declaration merging is when multiple declarations sharing the same name are automatically combined into a single definition by the compiler. Only `interface` supports this — declaring the same `interface` name twice merges their members; declaring the same `type` alias twice is a compile error.

<a id="how-would-you-make-all-properties-on-an-interface-optional-without-rewriting-each-one"></a>
### Q: How would you make all properties on an interface optional without rewriting each one?
**Answer:** Use the built-in `Partial<T>` utility type, which maps over every property of `T` and marks each one optional.

**Example:**
```ts
interface User { id: number; name: string; }
type PartialUser = Partial<User>;
```

<a id="can-a-type-alias-represent-a-union-or-a-primitive-and-can-an-interface"></a>
### Q: Can a `type` alias represent a union or a primitive, and can an `interface`?
**Answer:** A `type` alias can represent virtually anything — unions, intersections, primitives, tuples, function types — directly. An `interface` can only describe the shape of an object (including function/callable/constructable shapes), and cannot directly express a union or a bare primitive type on its own.

<a id="how-do-you-make-a-class-implement-an-interface-and-what-does-that-guarantee"></a>
### Q: How do you make a class implement an interface, and what does that guarantee?
**Answer:** Using the `implements` keyword — it guarantees the class provides at minimum the members (with compatible types) declared on the interface, checked at compile time; it doesn't automatically provide any implementation itself, only enforces the contract.

**Example:**
```ts
interface Greetable { greet(): string; }
class Person implements Greetable {
  greet() { return "Hello!"; }
}
```

<a id="what-are-index-signatures-and-when-would-you-use-one-on-an-interface"></a>
### Q: What are index signatures, and when would you use one on an interface?
**Answer:** An index signature (`[key: string]: SomeType`) describes an object whose exact property names aren't known upfront, but whose values all conform to a specific type — useful for describing dictionary-like or dynamically-keyed objects.

**Example:**
```ts
interface StringMap { [key: string]: string; }
```

<a id="what-are-optional-and-readonly-properties-on-an-interface"></a>
### Q: What are optional and readonly properties on an interface?
**Answer:** `prop?: Type` marks a property as not required to be present. `readonly prop: Type` allows the property to be read but not reassigned after the object is first created.

<a id="when-would-you-generally-prefer-type-over-interface-and-vice-versa"></a>
### Q: When would you generally prefer `type` over `interface`, and vice versa?
**Answer:** Prefer `interface` for object/class shapes meant to be extended or implemented, especially in public library APIs, since declaration merging can be genuinely useful there. Prefer `type` when you need unions, intersections, tuples, mapped types, or any type-level computation that `interface` simply can't express — many teams otherwise default to whichever is more idiomatic in their codebase's existing style.

---

<a id="functions"></a>
## Functions

<a id="how-do-you-type-a-functions-parameters-and-return-value"></a>
### Q: How do you type a function's parameters and return value?
**Answer:** Annotate each parameter with `: Type`, and the return type after the parameter list.

**Example:**
```ts
function add(a: number, b: number): number {
  return a + b;
}
```

<a id="what-is-an-optional-parameter-and-where-must-it-appear-in-the-parameter-list"></a>
### Q: What is an optional parameter, and where must it appear in the parameter list?
**Answer:** A parameter marked with `?` that can be omitted when calling the function; it becomes `undefined` if not provided. Optional parameters must come after all required parameters in the list.

<a id="what-is-a-default-parameter-and-how-does-it-interact-with-the-parameters-type"></a>
### Q: What is a default parameter, and how does it interact with the parameter's type?
**Answer:** A parameter given a default value (`function f(x: number = 10)`), used when the caller omits an argument (or passes `undefined`) for it. TypeScript automatically infers the parameter's type from the default value if no explicit annotation is given, and default parameters are implicitly treated as optional for callers.

<a id="how-do-you-type-rest-parameters"></a>
### Q: How do you type rest parameters?
**Answer:** Annotate them as an array type, since rest parameters collect any remaining arguments into an actual array.

**Example:**
```ts
function sum(...nums: number[]): number {
  return nums.reduce((a, b) => a + b, 0);
}
```

<a id="what-is-a-function-overload-in-typescript"></a>
### Q: What is a function overload in TypeScript?
**Answer:** Multiple declared signatures for the same function name, each describing a different valid combination of parameter/return types, followed by a single actual implementation whose signature is broad enough to cover all the declared overloads — lets callers get precise type checking for each specific calling pattern.

**Example:**
```ts
function format(value: string): string;
function format(value: number): string;
function format(value: string | number): string {
  return String(value);
}
```

<a id="what-is-the-difference-between-typing-a-function-with-an-arrow-function-type-vs-a-call-signature-in-an-interface"></a>
### Q: What is the difference between typing a function with an arrow function type vs. a call signature in an interface?
**Answer:** `type Fn = (x: number) => number;` and `interface Fn { (x: number): number; }` both describe the same callable shape — a call signature on an interface additionally allows adding extra properties to the same type (since a function is also an object in JS), which the simple arrow-type syntax can't express as directly.

<a id="how-does-typescript-type-this-inside-a-function-and-what-is-a-this-parameter"></a>
### Q: How does TypeScript type `this` inside a function, and what is a `this` parameter?
**Answer:** By default, `this` inside a regular function has an implicit `any` type unless `noImplicitThis` is enabled. You can explicitly declare the intended type of `this` as a fake first parameter (`function f(this: SomeType, ...)`), which TypeScript strips out at compile time but uses to type-check how the function is called.

<a id="what-is-a-generic-function-constraint-and-how-do-you-write-one"></a>
### Q: What is a generic function constraint, and how do you write one?
**Answer:** A constraint (`<T extends SomeType>`) restricts a generic type parameter to only types that satisfy `SomeType`, letting you safely access members of `SomeType` on values of type `T` inside the function body.

**Example:**
```ts
function getLength<T extends { length: number }>(item: T): number {
  return item.length;
}
```

---

<a id="classes--oop"></a>
## Classes & OOP

<a id="what-are-the-access-modifiers-in-typescript-classes-and-what-does-each-restrict"></a>
### Q: What are the access modifiers in TypeScript classes, and what does each restrict?
**Answer:** `public` (the default) — accessible from anywhere. `private` — accessible only from within the declaring class itself, not subclasses or outside code. `protected` — accessible within the declaring class and its subclasses, but not from outside code.

<a id="what-is-the-difference-between-typescripts-private-keyword-and-javascripts-native--private-fields"></a>
### Q: What is the difference between TypeScript's `private` keyword and JavaScript's native `#` private fields?
**Answer:** TypeScript's `private` is a compile-time-only restriction — it's fully erased in the compiled JavaScript output, so the property is still technically accessible at runtime (e.g. via bracket notation). JavaScript's native `#field` syntax is enforced by the JavaScript engine itself at runtime, providing true, unbypassable privacy even in the compiled output.

<a id="what-is-a-parameter-property-in-a-typescript-class-constructor"></a>
### Q: What is a parameter property in a TypeScript class constructor?
**Answer:** Adding an access modifier (`public`, `private`, `protected`, or `readonly`) directly to a constructor parameter automatically declares a class property with that name and assigns the parameter's value to it, without needing a separate property declaration and manual assignment.

**Example:**
```ts
class Point {
  constructor(public x: number, public y: number) {}
}
```

<a id="what-does-the-abstract-keyword-do-on-a-class-or-method"></a>
### Q: What does the `abstract` keyword do on a class or method?
**Answer:** An `abstract` class cannot be directly instantiated with `new` — it's meant to be extended. An `abstract` method has no implementation in the abstract class itself and must be implemented by any concrete subclass.

**Example:**
```ts
abstract class Shape {
  abstract area(): number;
}
```

<a id="how-does-typescript-type-static-properties-and-methods-and-how-are-they-accessed"></a>
### Q: How does TypeScript type static properties and methods, and how are they accessed?
**Answer:** Declared with the `static` keyword within the class body, and accessed via the class itself rather than an instance (`ClassName.staticMember`), just like in plain JavaScript — TypeScript adds type checking on top of that existing runtime behavior.

<a id="how-does-generics-apply-to-classes-in-typescript"></a>
### Q: How does generics apply to classes in TypeScript?
**Answer:** A class can declare its own type parameters (`class Box<T> { value: T; }`), letting instances of that class be specialized for a specific type when created (`new Box<string>()`), while the class's internal logic remains written generically once.

<a id="what-is-method-overriding-in-a-typescript-subclass-and-what-does-the-override-keyword-add"></a>
### Q: What is method overriding in a TypeScript subclass, and what does the `override` keyword add?
**Answer:** A subclass can redefine a method inherited from its parent class, replacing its implementation. The `override` keyword (added in TypeScript 4.3) explicitly marks that intent, and the compiler will error if you write `override` on a method that doesn't actually exist on the base class — catching typos or the base method being renamed/removed.

<a id="what-is-the-difference-between-an-interface-and-an-abstract-class-for-defining-a-contract"></a>
### Q: What is the difference between an interface and an abstract class for defining a contract?
**Answer:** An interface is purely a compile-time type contract with no implementation and no runtime footprint at all. An abstract class can provide actual shared implementation for some methods while still leaving others abstract, and it does exist as a real construct at runtime (usable with `instanceof`), unlike an interface.

<a id="what-are-getters-and-setters-in-a-typescript-class-and-how-are-they-typed"></a>
### Q: What are getters and setters in a TypeScript class, and how are they typed?
**Answer:** `get`/`set` accessor methods that let you run code when a property is read or assigned, while still using plain property-access syntax from the outside. Their types are inferred from the getter's return type and the setter's parameter type, and TypeScript checks that they're consistent with each other.

<a id="what-does-implementing-multiple-interfaces-on-a-single-class-look-like-and-does-typescript-support-multiple-inheritance-of-classes"></a>
### Q: What does implementing multiple interfaces on a single class look like, and does TypeScript support multiple inheritance of classes?
**Answer:** A class can implement several interfaces at once, comma-separated (`class Foo implements A, B {}`), since interfaces are just type contracts. TypeScript (like JavaScript) does not support extending multiple classes directly — a class can only `extend` one base class, though patterns like mixins can approximate multiple inheritance.

---

<a id="generics"></a>
## Generics

<a id="what-problem-do-generics-solve-that-any-doesnt"></a>
### Q: What problem do generics solve that `any` doesn't?
**Answer:** `any` disables type checking entirely, so you lose all information about a value's actual type. Generics preserve the specific type used at each call site, so the compiler can still enforce type safety and give you accurate autocompletion, while the underlying function/class logic remains reusable across many different types.

<a id="how-does-typescript-infer-generic-type-arguments-and-when-do-you-need-to-specify-them-explicitly"></a>
### Q: How does TypeScript infer generic type arguments, and when do you need to specify them explicitly?
**Answer:** TypeScript typically infers a generic parameter from the type(s) of the arguments actually passed to a call, e.g. `identity("hi")` infers `T` as `string` automatically. You need to specify explicitly (`identity<string>("hi")`) when there's nothing for the compiler to infer from, or when the inferred type would be wrong for what you actually intend.

<a id="what-is-a-generic-constraint-and-how-do-you-write-one-with-extends"></a>
### Q: What is a generic constraint, and how do you write one with `extends`?
**Answer:** `<T extends SomeShape>` restricts what types `T` is allowed to be — only types assignable to `SomeShape` — letting you safely rely on `SomeShape`'s members existing on any value of type `T` within the generic code.

<a id="what-are-default-generic-type-parameters"></a>
### Q: What are default generic type parameters?
**Answer:** A generic parameter can be given a default type, used when the caller doesn't explicitly specify one and the compiler also can't infer it from context.

**Example:**
```ts
interface ApiResponse<T = unknown> {
  data: T;
  status: number;
}
```

<a id="how-would-you-write-a-generic-function-that-works-on-any-array-and-returns-its-first-element"></a>
### Q: How would you write a generic function that works on any array and returns its first element?
**Answer:** Constrain or simply parameterize over the element type, since arrays are already generic (`T[]`).

**Example:**
```ts
function first<T>(arr: T[]): T | undefined {
  return arr[0];
}
```

<a id="what-is-the-difference-between-a-generic-type-parameter-used-on-a-function-versus-one-used-on-the-whole-classinterface"></a>
### Q: What is the difference between a generic type parameter used on a function versus one used on the whole class/interface?
**Answer:** A function-level generic parameter is scoped to that single function call, and can be inferred freshly each time it's called with different arguments. A class/interface-level generic parameter is fixed once for the entire instance/type when it's created, and every method within shares that same, single type argument.

<a id="what-is-keyof-t-combined-with-a-generic-used-for-eg-in-a-generic-get-property-function"></a>
### Q: What is `keyof T` combined with a generic used for, e.g. in a generic "get property" function?
**Answer:** It lets you write a strongly-typed function that accesses a property on an object by a dynamic key, while the compiler still verifies the key actually exists on that object and correctly infers the return type as the exact type of that property.

**Example:**
```ts
function getProp<T, K extends keyof T>(obj: T, key: K): T[K] {
  return obj[key];
}
```

<a id="what-are-variance-and-generic-type-parameter-positions-roughly-and-why-does-it-sometimes-matter-for-function-types"></a>
### Q: What are variance and generic type parameter positions (roughly), and why does it sometimes matter for function types?
**Answer:** Variance describes how subtyping relationships between complex types (like generics or function types) relate to the subtyping of their component types. It matters because a function that accepts a broader parameter type is still compatible where a function accepting a narrower one is expected (parameters are "contravariant"), while return types need to match the expected type or something narrower ("covariant") — TypeScript's structural type checker handles this mostly automatically, but it explains some otherwise-surprising compatibility errors with generic function types.

<a id="how-do-generics-interact-with-default-valuesinference-when-using-react-style-generic-components-or-hooks"></a>
### Q: How do generics interact with default values/inference when using React-style generic components or hooks?
**Answer:** A generic hook like `useState<T>()` lets you specify (or let TypeScript infer from an initial value) exactly what type of data that piece of state holds, so every subsequent read/write of that state is checked against that specific type, rather than being loosely typed or `any`.

<a id="what-is-a-conditional-type-used-together-with-generics-for-at-a-basic-level"></a>
### Q: What is a conditional type used together with generics for, at a basic level?
**Answer:** It lets a generic type's shape change based on a condition evaluated against another type, similar to an `if`/`else` but entirely at the type level, commonly written as `T extends U ? X : Y` — used heavily by TypeScript's own built-in utility types like `Exclude` and `ReturnType`.

---

<a id="union-intersection--literal-types"></a>
## Union, Intersection & Literal Types

<a id="how-do-you-narrow-a-union-type-using-typeof"></a>
### Q: How do you narrow a union type using `typeof`?
**Answer:** Check the runtime `typeof` of the value inside a conditional, and TypeScript automatically narrows the variable's type to match within that branch.

**Example:**
```ts
function print(value: string | number) {
  if (typeof value === "string") {
    console.log(value.toUpperCase()); // narrowed to string
  }
}
```

<a id="how-do-you-narrow-a-union-of-object-types-using-a-shared-discriminant-property"></a>
### Q: How do you narrow a union of object types using a shared discriminant property?
**Answer:** Give every member of the union a common property with a distinct literal value (like `kind` or `type`), then check that property in a conditional — TypeScript narrows to the exact matching member type based on which literal value matched.

<a id="what-happens-when-you-access-a-property-that-only-exists-on-some-members-of-a-union-type-without-narrowing-first"></a>
### Q: What happens when you access a property that only exists on some members of a union type, without narrowing first?
**Answer:** TypeScript raises a compile error, since the property isn't guaranteed to exist on every possible member of the union — you must narrow the type first (with a type guard) before safely accessing a member-specific property.

<a id="what-is-the-difference-between-a-union-type-and-an-enum-for-representing-a-fixed-set-of-options"></a>
### Q: What is the difference between a union type and an enum for representing a fixed set of options?
**Answer:** A union of string literal types (`"a" | "b" | "c"`) exists purely at the type level with zero runtime footprint. An `enum` creates an actual runtime object (unless declared `const enum`) that exists in the compiled JavaScript output, and can be referenced by name at runtime, not just used as a compile-time type.

<a id="how-do-intersection-types-behave-when-combining-two-object-types-with-a-property-of-the-same-name-but-incompatible-types"></a>
### Q: How do intersection types behave when combining two object types with a property of the same name but incompatible types?
**Answer:** The resulting property's type becomes the intersection of both individual types, which for genuinely incompatible primitive types (like `string & number`) collapses to `never` — meaning no valid value could ever satisfy that property, effectively making the object impossible to construct.

<a id="what-is-a-nullable-union-type-and-how-do-you-safely-work-with-one-under-strictnullchecks"></a>
### Q: What is a nullable union type, and how do you safely work with one under `strictNullChecks`?
**Answer:** A type like `string | null` (or `| undefined`) that explicitly allows the value to be missing. You safely work with it by narrowing first — an `if (value !== null)` check, optional chaining (`value?.length`), or a nullish coalescing default (`value ?? "default"`).

<a id="can-you-use-a-union-type-as-a-function-parameter-and-what-are-the-implications-for-the-function-body"></a>
### Q: Can you use a union type as a function parameter, and what are the implications for the function body?
**Answer:** Yes — but inside the function body, you're generally restricted to only the members/operations common to every type in the union, unless you narrow the parameter with a type guard first to work with one specific member type at a time.

<a id="what-is-an-exhaustiveness-check-using-never-and-why-is-it-useful-with-discriminated-unions"></a>
### Q: What is an exhaustiveness check using `never`, and why is it useful with discriminated unions?
**Answer:** In a `switch` statement over a discriminated union, assigning the unhandled value to a variable typed as `never` in the `default` case causes a compile error if any union member isn't explicitly handled — a safeguard that automatically flags forgotten cases if the union is later extended with a new member.

**Example:**
```ts
function assertNever(x: never): never {
  throw new Error("Unhandled case: " + x);
}
```

---

<a id="advanced--utility-types"></a>
## Advanced & Utility Types

<a id="what-does-partialt-do"></a>
### Q: What does `Partial<T>` do?
**Answer:** Produces a new type with every property of `T` made optional — useful for things like an "update" function that only needs to accept a subset of an object's fields.

<a id="what-does-pickt-k-and-omitt-k-do"></a>
### Q: What does `Pick<T, K>` and `Omit<T, K>` do?
**Answer:** `Pick<T, K>` produces a new type containing only the specified subset of properties `K` from `T`. `Omit<T, K>` produces a new type containing everything from `T` except the specified properties `K` — the inverse operation.

<a id="what-does-recordk-v-do-and-when-is-it-useful"></a>
### Q: What does `Record<K, V>` do, and when is it useful?
**Answer:** It constructs an object type whose keys are all of type `K` and whose values are all of type `V` — commonly used for typing dictionary/lookup-style objects.

**Example:**
```ts
type Scores = Record<string, number>;
```

<a id="what-does-returntypet-do-and-what-is-a-common-use-case"></a>
### Q: What does `ReturnType<T>` do, and what is a common use case?
**Answer:** It extracts the return type of a given function type as a standalone type, without you needing to manually write it out separately — useful for keeping a derived type automatically in sync with a function's actual, possibly-inferred return type.

<a id="what-is-a-mapped-type-and-how-would-you-write-a-simplified-version-of-readonlyt-yourself"></a>
### Q: What is a mapped type, and how would you write a simplified version of `Readonly<T>` yourself?
**Answer:** A mapped type iterates over the properties of an existing type to produce a new, transformed type, using a syntax similar to an index signature but iterating with `in keyof`.

**Example:**
```ts
type MyReadonly<T> = {
  readonly [K in keyof T]: T[K];
};
```

<a id="what-is-a-conditional-type-and-how-does-infer-work-within-one"></a>
### Q: What is a conditional type, and how does `infer` work within one?
**Answer:** A conditional type (`T extends U ? X : Y`) selects between two types based on whether `T` is assignable to `U`. The `infer` keyword, used within the `extends` clause, lets you capture and name a type that TypeScript would otherwise only check for, making it usable in the resulting type — this is how utility types like `ReturnType<T>` are actually implemented internally.

**Example:**
```ts
type MyReturnType<T> = T extends (...args: any[]) => infer R ? R : never;
```

<a id="what-does-requiredt-do-and-how-does-it-differ-from-partialt"></a>
### Q: What does `Required<T>` do, and how does it differ from `Partial<T>`?
**Answer:** `Required<T>` makes every property of `T` mandatory, removing any `?` optional modifiers — the exact opposite transformation of `Partial<T>`, which makes every property optional.

<a id="what-is-a-distributive-conditional-type"></a>
### Q: What is a distributive conditional type?
**Answer:** When a conditional type's checked type is a bare, naked type parameter and you pass in a union, TypeScript automatically applies the conditional to each union member individually and combines the results back into a union — this default "distributive" behavior is why `Exclude<T, U>` works correctly across every member of a union passed as `T`.

<a id="what-does-excludet-u-and-extractt-u-do"></a>
### Q: What does `Exclude<T, U>` and `Extract<T, U>` do?
**Answer:** `Exclude<T, U>` produces a type with every member of union `T` that's assignable to `U` removed. `Extract<T, U>` does the opposite — it keeps only the members of `T` that are assignable to `U`.

<a id="what-is-the-difference-between-awaitedt-and-just-accessing-the-resolved-type-of-a-promise-manually"></a>
### Q: What is the difference between `Awaited<T>` and just accessing the resolved type of a `Promise` manually?
**Answer:** `Awaited<T>` (added in TypeScript 4.5) correctly unwraps a `Promise<T>` down to its resolved value type, and — unlike a naive manual approach — also correctly handles nested/chained promises (a `Promise` that resolves to another `Promise`), recursively unwrapping until it reaches a non-promise type, mirroring what `await` actually does at runtime.

---

<a id="type-narrowing--guards"></a>
## Type Narrowing & Guards

<a id="what-is-the-in-operator-used-for-as-a-type-guard"></a>
### Q: What is the `in` operator used for as a type guard?
**Answer:** It checks whether a specific property name exists on an object at runtime, and TypeScript uses that check to narrow a union of object types down to the specific member(s) that actually declare that property.

**Example:**
```ts
function move(pet: Fish | Bird) {
  if ("swim" in pet) pet.swim();
  else pet.fly();
}
```

<a id="what-is-the-instanceof-operator-used-for-as-a-type-guard-and-what-kind-of-types-does-it-work-with"></a>
### Q: What is the `instanceof` operator used for as a type guard, and what kind of types does it work with?
**Answer:** It checks whether a value was constructed by a specific class (or one of its subclasses) at runtime, and TypeScript narrows the value's type accordingly. It only works with class instances, not plain object shapes defined by `interface`/`type` alone, since interfaces have no runtime representation to check against.

<a id="how-does-typescript-narrow-a-type-based-on-a-truthy-check-eg-if-value"></a>
### Q: How does TypeScript narrow a type based on a truthy check, e.g. `if (value)`?
**Answer:** It excludes falsy possibilities from the type within that branch — `null`, `undefined`, `0`, `""`, `false`, and `NaN` — narrowing e.g. `string | null | undefined` down to just `string` inside an `if (value)` block.

<a id="what-is-a-user-defined-type-predicate-function-and-what-makes-its-signature-special"></a>
### Q: What is a user-defined type predicate function, and what makes its signature special?
**Answer:** A function whose return type is written as `value is SomeType` instead of a plain `boolean`. Even though it returns a normal boolean at runtime, TypeScript treats calling it in a conditional as a genuine type guard, narrowing the checked variable's type in the branch where the function returned `true`.

<a id="how-does-typescript-narrow-within-an-else-branch-or-after-an-early-return"></a>
### Q: How does TypeScript narrow within an `else` branch, or after an early `return`?
**Answer:** The compiler tracks control flow throughout the function — if an `if` branch returns, throws, or otherwise can't fall through, TypeScript narrows the type in the code that follows as if that branch's condition were false, without needing an explicit `else`.

<a id="what-is-the-difference-between-narrowing-with--versus--against-null"></a>
### Q: What is the difference between narrowing with `==`/`!=` versus `===`/`!==` against `null`?
**Answer:** `value == null` checks for both `null` and `undefined` simultaneously (due to JavaScript's loose equality quirks with `null`), which TypeScript recognizes and narrows accordingly. `value === null` checks only for `null` specifically, leaving `undefined` still a possibility in the narrowed type.

<a id="can-you-narrow-a-type-using-a-value-stored-in-a-variable-rather-than-an-inline-condition-eg-assigning-const-isstring--typeof-x--string-first"></a>
### Q: Can you narrow a type using a value stored in a variable rather than an inline condition, e.g. assigning `const isString = typeof x === "string"` first?
**Answer:** Historically this was a common limitation — TypeScript couldn't narrow based on a boolean stored in a separate variable. As of TypeScript 4.4+, control-flow analysis of aliased conditions allows this for `const` variables (and readonly properties) holding a type-guard expression, letting the narrowing persist through the alias.

<a id="what-is-assertion-based-narrowing-with-asserts-functions-and-how-does-it-differ-from-a-type-predicate-function"></a>
### Q: What is assertion-based narrowing with `asserts` functions, and how does it differ from a type predicate function?
**Answer:** A type predicate function (`value is T`) narrows the type within the branch where it was checked and returned true. An `asserts` function (`function assert(value: unknown): asserts value is T`) instead throws if the assertion fails, and if it doesn't throw, TypeScript narrows the type for the rest of the enclosing scope from that point forward, not just within a conditional branch.

---

<a id="enums"></a>
## Enums

<a id="what-is-an-enum-in-typescript-and-what-does-it-compile-down-to-by-default"></a>
### Q: What is an enum in TypeScript, and what does it compile down to by default?
**Answer:** A named set of related constant values. A regular (non-const) numeric enum compiles to an actual JavaScript object at runtime, with both a forward mapping (name → value) and, for numeric enums, a reverse mapping (value → name).

**Example:**
```ts
enum Direction { Up, Down, Left, Right }
```

<a id="what-is-the-difference-between-a-numeric-enum-and-a-string-enum"></a>
### Q: What is the difference between a numeric enum and a string enum?
**Answer:** A numeric enum auto-assigns increasing numbers starting at 0 (unless explicitly set), and generates a reverse value-to-name mapping at runtime. A string enum requires each member to be explicitly initialized with a string value, and does not generate any reverse mapping.

<a id="what-is-a-const-enum-and-how-does-it-differ-from-a-regular-enum-at-compile-time"></a>
### Q: What is a `const enum`, and how does it differ from a regular enum at compile time?
**Answer:** A `const enum` is fully inlined at every usage site during compilation and produces no actual runtime object at all, resulting in smaller and faster compiled output — the trade-off is it can't be used with certain tools/bundlers that need the actual runtime object to exist (like isolated file transpilation without full type information).

<a id="what-are-some-common-criticisms-of-enums-and-what-alternative-do-many-teams-prefer"></a>
### Q: What are some common criticisms of enums, and what alternative do many teams prefer?
**Answer:** Enums are one of the few TypeScript features that aren't just erased plain JavaScript — they generate actual runtime code with some quirky behaviors (like numeric enums' reverse mapping), and don't always play perfectly with tree-shaking or certain build tools. Many teams prefer a union of string literal types (`type Direction = "up" | "down"`) instead, which has zero runtime footprint and behaves more predictably.

<a id="can-you-assign-a-plain-number-directly-to-a-numeric-enum-typed-variable"></a>
### Q: Can you assign a plain number directly to a numeric enum-typed variable?
**Answer:** Yes — numeric enums are structurally compatible with the `number` type, so any `number` value can be assigned to a variable typed with a numeric enum, even if it doesn't correspond to any of the enum's declared members, which is another commonly cited weak point of numeric enums' type safety.

<a id="how-would-you-iterate-over-the-members-of-a-string-enum"></a>
### Q: How would you iterate over the members of a string enum?
**Answer:** Since a string enum's runtime object only has a forward mapping (no reverse mapping like numeric enums), you can use `Object.values(EnumName)` to get an array of its actual string values.

---

<a id="modules--namespaces"></a>
## Modules & Namespaces

<a id="what-is-the-difference-between-an-es-module-and-a-typescript-namespace"></a>
### Q: What is the difference between an ES module and a TypeScript namespace?
**Answer:** ES modules (`import`/`export`) are the standard JavaScript module system, with each file being its own scope, and are the generally recommended approach today. Namespaces (`namespace Foo { ... }`) are an older, TypeScript-specific way to group and organize code under a shared global-ish name, largely superseded by ES modules for most modern project structures.

<a id="what-is-the-difference-between-a-default-export-and-a-named-export-in-typescript"></a>
### Q: What is the difference between a default export and a named export in TypeScript?
**Answer:** Functionally identical to plain JavaScript's module system — a file can have one default export, imported under any name, and any number of named exports, imported with matching names in curly braces; TypeScript adds full type checking on top of both.

<a id="what-does-export-type-a-type-only-export-do-and-why-would-you-use-it"></a>
### Q: What does `export type` (a type-only export) do, and why would you use it?
**Answer:** It explicitly marks an export as being type information only, with no runtime value, letting build tools safely strip it out entirely during compilation — useful for guaranteeing a particular import doesn't accidentally pull in runtime code when only type information was actually needed.

<a id="what-is-module-augmentation-and-what-is-it-used-for"></a>
### Q: What is module augmentation, and what is it used for?
**Answer:** A pattern for adding new members to an existing module's exported types from a separate file — commonly used to extend a third-party library's types (e.g. adding a custom property to Express's `Request` type) without modifying that library's own source code.

<a id="what-is-the-difference-between-import-type-and-a-regular-import"></a>
### Q: What is the difference between `import type` and a regular `import`?
**Answer:** `import type` explicitly imports only type information, guaranteed to be fully erased at compile time with no runtime side effects (like triggering the imported module's top-level code to execute) — useful for avoiding circular import issues or unnecessary runtime dependencies when only a type is actually needed.

<a id="what-is-a-barrel-file-and-whats-a-potential-downside-of-using-one"></a>
### Q: What is a barrel file, and what's a potential downside of using one?
**Answer:** A file (commonly `index.ts`) that re-exports members from several other files in a directory, letting consumers import from one single, convenient path. A downside is it can hurt tree-shaking (since bundlers may struggle to determine which specific re-exported pieces are actually used) and can slow down TypeScript's own type-checking in very large projects with many barrel files.

---

<a id="decorators"></a>
## Decorators

<a id="what-is-a-decorator-in-typescript-and-what-does-it-let-you-do"></a>
### Q: What is a decorator in TypeScript, and what does it let you do?
**Answer:** A special kind of declaration, written with an `@expression` syntax, that can be attached to a class, method, property, or parameter to observe, modify, or replace its definition at the point it's declared — commonly used for things like logging, validation, or dependency injection metadata.

<a id="what-is-the-difference-between-a-class-decorator-and-a-method-decorator"></a>
### Q: What is the difference between a class decorator and a method decorator?
**Answer:** A class decorator receives the class's constructor itself and can inspect, modify, or even return a replacement constructor. A method decorator receives the class's prototype, the method's name, and its property descriptor, letting it wrap or replace the method's actual implementation.

<a id="how-do-you-enable-decorators-in-a-typescript-project-and-why-arent-they-on-by-default"></a>
### Q: How do you enable decorators in a TypeScript project, and why aren't they on by default?
**Answer:** Set `"experimentalDecorators": true` in `tsconfig.json` for the older, widely-used decorator implementation (as used by frameworks like Angular and NestJS). They weren't enabled by default historically because the proposal was still evolving in the JavaScript standards process, and TypeScript's implementation predates the now-finalized ECMAScript decorators standard, which TypeScript has since also added separate support for.

<a id="what-is-a-decorator-factory"></a>
### Q: What is a decorator factory?
**Answer:** A function that returns a decorator function, letting you pass configuration/arguments to customize the decorator's behavior at the point it's applied, rather than the decorator always behaving identically everywhere it's used.

**Example:**
```ts
function Log(prefix: string) {
  return function (target: any, key: string, descriptor: PropertyDescriptor) {
    // use `prefix` inside here
  };
}
```

<a id="what-is-reflect-metadata-and-how-does-it-relate-to-decorators-in-frameworks-like-nestjs"></a>
### Q: What is `reflect-metadata`, and how does it relate to decorators in frameworks like NestJS?
**Answer:** A library that lets decorators attach and later retrieve arbitrary metadata associated with a class or its members at runtime — frameworks like NestJS and Angular use this heavily for dependency injection, reading metadata (like parameter types) that decorators recorded to automatically figure out what to inject where.

<a id="what-order-do-multiple-decorators-applied-to-the-same-declaration-run-in"></a>
### Q: What order do multiple decorators applied to the same declaration run in?
**Answer:** Their "factory" expressions are evaluated top-to-bottom, but the actual decorator functions themselves are then applied bottom-to-top (closest to the declaration first) — similar in principle to function composition.

---

<a id="tsconfig--tooling"></a>
## tsconfig & Tooling

<a id="what-is-tsconfigjson-and-what-is-its-basic-purpose"></a>
### Q: What is `tsconfig.json`, and what is its basic purpose?
**Answer:** A configuration file at the root of a TypeScript project specifying which files to include/exclude from compilation, the compiler options to use (target JS version, module system, strictness flags, output directory, etc.), and project-wide settings.

<a id="what-does-the-target-compiler-option-control"></a>
### Q: What does the `target` compiler option control?
**Answer:** Which version of JavaScript the TypeScript compiler outputs — e.g. `ES2015` or `ES2020` — determining whether newer JS syntax (like optional chaining or classes) is left as-is or transpiled down into older, more broadly compatible syntax.

<a id="what-does-the-module-compiler-option-control"></a>
### Q: What does the `module` compiler option control?
**Answer:** Which module system the compiled output uses for `import`/`export` statements — e.g. `CommonJS` (Node.js's `require`), `ESNext` (native ES modules), or others — needs to match whatever your runtime/bundler actually expects.

<a id="what-is-the-difference-between-noimplicitany-and-strict"></a>
### Q: What is the difference between `noImplicitAny` and `strict`?
**Answer:** `noImplicitAny` specifically errors when a type can't be inferred and would otherwise silently default to `any`. `strict` is a broader flag that enables `noImplicitAny` along with several other stricter checks (like `strictNullChecks`) all at once.

<a id="what-does-esmoduleinterop-do-and-what-problem-does-it-solve"></a>
### Q: What does `esModuleInterop` do, and what problem does it solve?
**Answer:** It enables a compatibility shim allowing cleaner default-import syntax (`import React from "react"`) when importing CommonJS modules that don't have a real ES-module-style default export, avoiding the more awkward `import * as React from "react"` syntax that was otherwise technically required.

<a id="what-is-the-difference-between-tsc---noemit-and-a-regular-tsc-build"></a>
### Q: What is the difference between `tsc --noEmit` and a regular `tsc` build?
**Answer:** A regular `tsc` build type-checks the project AND writes out compiled `.js` files. `tsc --noEmit` only performs type checking, producing no output files at all — commonly used in CI pipelines or editor tooling purely to verify there are no type errors, when a separate tool (like Babel or esbuild) handles the actual JS transpilation.

<a id="what-does-the-skiplibcheck-option-do-and-why-might-a-project-enable-it"></a>
### Q: What does the `skipLibCheck` option do, and why might a project enable it?
**Answer:** It skips type-checking of all `.d.ts` declaration files, including those from `node_modules`, only type-checking your own project's source files. It's commonly enabled to speed up compilation and avoid unrelated type errors originating from third-party libraries' own (sometimes imperfect) type definitions.

<a id="what-is-the-difference-between-using-tsc-directly-versus-a-tool-like-babel-esbuild-or-swc-to-compile-typescript"></a>
### Q: What is the difference between using `tsc` directly versus a tool like Babel, esbuild, or SWC to compile TypeScript?
**Answer:** `tsc` performs both type checking and JavaScript emission together. Tools like Babel, esbuild, and SWC can strip TypeScript's type annotations and compile the code much faster, but they do so file-by-file without actually checking types at all — meaning type checking has to be run as a wholly separate step (e.g. `tsc --noEmit`) alongside them if you still want that safety net.

---

<a id="behavioral--scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="youre-converting-a-large-existing-javascript-codebase-to-typescript--how-would-you-approach-it"></a>
### Q: You're converting a large existing JavaScript codebase to TypeScript — how would you approach it?
**Answer:** Start by enabling `allowJs` and `checkJs` (or just `allowJs`) so TypeScript and JavaScript files can coexist, incrementally rename files from `.js` to `.ts` starting with the most foundational/shared modules, initially keep `strict` mode off (or use `// @ts-nocheck` sparingly) to avoid being overwhelmed, then progressively tighten strictness flags and eliminate `any` usages as the migration matures.

<a id="a-third-party-javascript-library-you-depend-on-has-no-official-typescript-types--how-would-you-handle-it"></a>
### Q: A third-party JavaScript library you depend on has no official TypeScript types — how would you handle it?
**Answer:** Check if community-maintained types exist under the `@types/` namespace on npm (DefinitelyTyped) and install those first. If none exist, write a minimal custom `.d.ts` declaration file describing just the parts of the library's API you actually use, or as a last resort, declare the module loosely with `declare module "library-name";` to silence errors while treating it as `any`.

<a id="a-colleague-keeps-using-any-to-quickly-silence-type-errors-instead-of-fixing-them-properly--how-would-you-address-this-in-a-code-review"></a>
### Q: A colleague keeps using `any` to quickly silence type errors instead of fixing them properly — how would you address this in a code review?
**Answer:** Point out that `any` disables type checking entirely for that value going forward, potentially hiding real bugs rather than fixing them, and suggest `unknown` with proper narrowing, or a more accurate specific type, as safer alternatives — while acknowledging `any` occasionally has legitimate, deliberate uses (like gradually migrating legacy code) that are worth distinguishing from just avoiding the real fix.

<a id="youre-seeing-a-confusing-typescript-error-about-incompatible-types-that-doesnt-clearly-explain-the-actual-problem--how-would-you-debug-it"></a>
### Q: You're seeing a confusing TypeScript error about incompatible types that doesn't clearly explain the actual problem — how would you debug it?
**Answer:** Hover over the specific variables involved in an editor to check their actual inferred types, break a large complex expression into smaller intermediate variables with explicit type annotations to isolate exactly where the mismatch originates, and check whether a structural typing quirk (like excess property checks or variance in function types) is the real underlying cause rather than the surface-level error message.

<a id="how-would-you-decide-whether-to-model-a-piece-of-state-as-a-union-of-string-literals-versus-an-enum"></a>
### Q: How would you decide whether to model a piece of state as a union of string literals versus an enum?
**Answer:** Default to a union of string literals for most cases, since it has zero runtime footprint, serializes cleanly to JSON, and integrates simply with most tooling. Consider an enum specifically if you need an actual runtime-iterable set of named constants, or the team's existing codebase/conventions already lean on enums consistently elsewhere.

<a id="how-would-you-type-an-api-response-where-the-shape-isnt-fully-guaranteed-to-match-your-typescript-types-at-runtime"></a>
### Q: How would you type an API response where the shape isn't fully guaranteed to match your TypeScript types at runtime?
**Answer:** Recognize that TypeScript types alone provide zero runtime protection — the network response could always diverge from what you declared. Use a runtime validation library (like Zod or io-ts) to actually parse and verify the response's shape against a schema at runtime, and derive your static TypeScript type from that same schema so both stay automatically in sync.

<a id="how-would-you-approach-reviewing-a-pull-request-that-introduces-a-lot-of-new-generic-types-you-find-hard-to-follow"></a>
### Q: How would you approach reviewing a pull request that introduces a lot of new generic types you find hard to follow?
**Answer:** Ask the author whether the complexity is genuinely necessary for the problem being solved, or whether a simpler, more concrete type would cover the actual use cases just as well; suggest adding a short comment explaining the generic's intent where it's non-obvious, and check whether the added complexity is actually catching real bugs or just adding friction without meaningful safety benefit.

<a id="a-generic-utility-function-you-wrote-type-checks-fine-but-produces-confusing-autocompletehover-types-for-consumers--how-would-you-improve-it"></a>
### Q: A generic utility function you wrote type-checks fine but produces confusing autocomplete/hover types for consumers — how would you improve it?
**Answer:** Consider whether intermediate mapped/conditional types are needlessly complex and could be simplified, add named helper types with clear names instead of deeply nested inline type expressions, and test the actual hover/autocomplete experience in an editor as you iterate, since a type that "type-checks correctly" isn't the same as one that's pleasant and clear for other developers actually using it.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to advanced types and tooling.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
