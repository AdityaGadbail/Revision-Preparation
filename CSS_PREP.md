# CSS Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of CSS interview questions — from fundamentals to layout systems, animations, and architecture — with clear answers and code examples where they help. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions)
  - [What is CSS specificity, and how is it calculated?](#what-is-css-specificity-and-how-is-it-calculated)
  - [What is margin collapsing, and when does it happen?](#what-is-margin-collapsing-and-when-does-it-happen)
  - [What is the difference between `display: none` and `visibility: hidden`?](#what-is-the-difference-between-display-none-and-visibility-hidden)
  - [What is the box model, and what does `box-sizing: border-box` change about it?](#what-is-the-box-model-and-what-does-box-sizing-border-box-change-about-it)
  - [What is the difference between `relative`, `absolute`, `fixed`, and `sticky` positioning?](#what-is-the-difference-between-relative-absolute-fixed-and-sticky-positioning)
  - [What is the difference between `em`, `rem`, `%`, and `px` units?](#what-is-the-difference-between-em-rem-and-px-units)
  - [What is the difference between Flexbox and Grid, and when would you use each?](#what-is-the-difference-between-flexbox-and-grid-and-when-would-you-use-each)
  - [Why doesn't `height: 100%` always work as expected?](#why-doesnt-height-100-always-work-as-expected)
  - [What is the CSS cascade, and how does it decide which styles apply?](#what-is-the-css-cascade-and-how-does-it-decide-which-styles-apply)
  - [What does `!important` do, and why is it generally discouraged?](#what-does-important-do-and-why-is-it-generally-discouraged)
  - [What is the difference between `inline`, `block`, and `inline-block` display values?](#what-is-the-difference-between-inline-block-and-inline-block-display-values)
  - [How does `z-index` work, and why doesn't it always behave as expected?](#how-does-z-index-work-and-why-doesnt-it-always-behave-as-expected)
  - [What is the difference between `:hover` and `:focus`, and why do both matter?](#what-is-the-difference-between-hover-and-focus-and-why-do-both-matter)
  - [What is a CSS reset or normalize, and why use one?](#what-is-a-css-reset-or-normalize-and-why-use-one)
  - [What is the difference between `min-width`/`max-width` and `width`?](#what-is-the-difference-between-min-widthmax-width-and-width)
  - [What is a stacking context, and what commonly creates one by surprise?](#what-is-a-stacking-context-and-what-commonly-creates-one-by-surprise)
- [CSS Basics](#css-basics)
  - [What is CSS, and what problem does it solve?](#what-is-css-and-what-problem-does-it-solve)
  - [What are the three ways to add CSS to an HTML page?](#what-are-the-three-ways-to-add-css-to-an-html-page)
  - [What is the basic syntax of a CSS rule?](#what-is-the-basic-syntax-of-a-css-rule)
  - [What is the difference between a class selector and an id selector?](#what-is-the-difference-between-a-class-selector-and-an-id-selector)
  - [How do you write CSS comments?](#how-do-you-write-css-comments)
  - [What is the difference between shorthand and longhand CSS properties?](#what-is-the-difference-between-shorthand-and-longhand-css-properties)
  - [What is the difference between absolute and relative CSS units?](#what-is-the-difference-between-absolute-and-relative-css-units)
  - [What is the difference between `color`, `background-color`, and `border-color`?](#what-is-the-difference-between-color-background-color-and-border-color)
  - [How do you apply a CSS rule to multiple selectors at once?](#how-do-you-apply-a-css-rule-to-multiple-selectors-at-once)
  - [Where is `!important` placed in a declaration?](#where-is-important-placed-in-a-declaration)
  - [What is the difference between `content-box` and `border-box` in `box-sizing`?](#what-is-the-difference-between-content-box-and-border-box-in-box-sizing)
  - [What is the difference between `inherit`, `initial`, and `unset` as CSS values?](#what-is-the-difference-between-inherit-initial-and-unset-as-css-values)
- [Selectors & Specificity](#selectors-specificity)
  - [What is the difference between a descendant selector and a child selector?](#what-is-the-difference-between-a-descendant-selector-and-a-child-selector)
  - [What is the difference between the adjacent sibling (+) and general sibling (~) combinators?](#what-is-the-difference-between-the-adjacent-sibling-and-general-sibling-combinators)
  - [What are attribute selectors, and how do you use them?](#what-are-attribute-selectors-and-how-do-you-use-them)
  - [What is the universal selector, and when is it used?](#what-is-the-universal-selector-and-when-is-it-used)
  - [What is the difference between a pseudo-class and a pseudo-element?](#what-is-the-difference-between-a-pseudo-class-and-a-pseudo-element)
  - [How is specificity calculated, step by step?](#how-is-specificity-calculated-step-by-step)
  - [What is the difference between `:nth-child()` and `:nth-of-type()`?](#what-is-the-difference-between-nth-child-and-nth-of-type)
  - [What does the `:not()` pseudo-class do?](#what-does-the-not-pseudo-class-do)
  - [What is the difference between `:first-child` and `:first-of-type`?](#what-is-the-difference-between-first-child-and-first-of-type)
  - [Does selector order or structure affect matching performance?](#does-selector-order-or-structure-affect-matching-performance)
  - [What is the `:is()` (and `:where()`) selector, and what problem does it solve?](#what-is-the-is-and-where-selector-and-what-problem-does-it-solve)
  - [What is the difference between `.class1.class2` and `.class1 .class2` as selectors?](#what-is-the-difference-between-class1class2-and-class1-class2-as-selectors)
- [Box Model & Layout](#box-model-layout)
  - [What are the four parts of the CSS box model, from inside out?](#what-are-the-four-parts-of-the-css-box-model-from-inside-out)
  - [What is the difference between margin and padding?](#what-is-the-difference-between-margin-and-padding)
  - [What causes margin collapsing, and how do you prevent it?](#what-causes-margin-collapsing-and-how-do-you-prevent-it)
  - [What is a Block Formatting Context (BFC), and why does it matter?](#what-is-a-block-formatting-context-bfc-and-why-does-it-matter)
  - [What is the difference between `overflow: visible`, `hidden`, `scroll`, and `auto`?](#what-is-the-difference-between-overflow-visible-hidden-scroll-and-auto)
  - [How do you horizontally and vertically center a block element?](#how-do-you-horizontally-and-vertically-center-a-block-element)
  - [What is the difference between `width: 100%` and `width: 100vw`?](#what-is-the-difference-between-width-100-and-width-100vw)
  - [What are floats, and what were they historically used for?](#what-are-floats-and-what-were-they-historically-used-for)
  - [What is the "clearfix" technique, and why was it needed?](#what-is-the-clearfix-technique-and-why-was-it-needed)
  - [What is the difference between `visibility: collapse` and `display: none` for table rows?](#what-is-the-difference-between-visibility-collapse-and-display-none-for-table-rows)
- [Flexbox](#flexbox)
  - [What is Flexbox, and what problem does it solve?](#what-is-flexbox-and-what-problem-does-it-solve)
  - [What is the difference between the main axis and the cross axis in Flexbox?](#what-is-the-difference-between-the-main-axis-and-the-cross-axis-in-flexbox)
  - [What do `flex-grow`, `flex-shrink`, and `flex-basis` each control?](#what-do-flex-grow-flex-shrink-and-flex-basis-each-control)
  - [What does `justify-content` control, and what are its common values?](#what-does-justify-content-control-and-what-are-its-common-values)
  - [What does `align-items` control, versus `align-content`?](#what-does-align-items-control-versus-align-content)
  - [What does `align-self` do, and how does it differ from `align-items`?](#what-does-align-self-do-and-how-does-it-differ-from-align-items)
  - [What is the shorthand `flex` property, and what does `flex: 1` mean?](#what-is-the-shorthand-flex-property-and-what-does-flex-1-mean)
  - [What does `flex-wrap` do, and what's the difference between `wrap` and `nowrap`?](#what-does-flex-wrap-do-and-whats-the-difference-between-wrap-and-nowrap)
  - [How do you reverse the order of flex items without changing the HTML?](#how-do-you-reverse-the-order-of-flex-items-without-changing-the-html)
  - [How would you build a classic "sticky footer" layout using Flexbox?](#how-would-you-build-a-classic-sticky-footer-layout-using-flexbox)
- [Grid](#grid)
  - [What is CSS Grid, and how does it differ from Flexbox?](#what-is-css-grid-and-how-does-it-differ-from-flexbox)
  - [How do you define columns and rows in a Grid container?](#how-do-you-define-columns-and-rows-in-a-grid-container)
  - [What is the `fr` unit in Grid, and how does it work?](#what-is-the-fr-unit-in-grid-and-how-does-it-work)
  - [What is the difference between `grid-template-areas` and manually placing items with line numbers?](#what-is-the-difference-between-grid-template-areas-and-manually-placing-items-with-line-numbers)
  - [What does `repeat()` do in a `grid-template-columns` declaration?](#what-does-repeat-do-in-a-grid-template-columns-declaration)
  - [What is the difference between `auto-fill` and `auto-fit` in `repeat()`?](#what-is-the-difference-between-auto-fill-and-auto-fit-in-repeat)
  - [What do `grid-column` and `grid-row` shorthand properties do?](#what-do-grid-column-and-grid-row-shorthand-properties-do)
  - [What is the `gap` property (and `row-gap`/`column-gap`) in Grid/Flexbox?](#what-is-the-gap-property-and-row-gapcolumn-gap-in-gridflexbox)
  - [How would you build a responsive grid without using media queries?](#how-would-you-build-a-responsive-grid-without-using-media-queries)
  - [What is the difference between implicit and explicit grid tracks?](#what-is-the-difference-between-implicit-and-explicit-grid-tracks)
- [Positioning & Display](#positioning-display)
  - [What are the possible values of the `position` property, and what does each do?](#what-are-the-possible-values-of-the-position-property-and-what-does-each-do)
  - [What is a "positioned ancestor," and why does it matter for absolute positioning?](#what-is-a-positioned-ancestor-and-why-does-it-matter-for-absolute-positioning)
  - [What is the difference between `display: none` and `opacity: 0`?](#what-is-the-difference-between-display-none-and-opacity-0)
  - [How does `position: sticky` actually work, and what's a common gotcha?](#how-does-position-sticky-actually-work-and-whats-a-common-gotcha)
  - [What is the difference between `display: inline-block` and `float` for laying out elements side by side?](#what-is-the-difference-between-display-inline-block-and-float-for-laying-out-elements-side-by-side)
  - [What is a stacking context, and what creates one?](#what-is-a-stacking-context-and-what-creates-one)
  - [What is the difference between `top`/`right`/`bottom`/`left` on a `static` vs. `relative`/`absolute` element?](#what-is-the-difference-between-toprightbottomleft-on-a-static-vs-relativeabsolute-element)
  - [What does `display: contents` do?](#what-does-display-contents-do)
  - [What is the difference between `visibility: hidden` and `display: none` in terms of transitions/animations?](#what-is-the-difference-between-visibility-hidden-and-display-none-in-terms-of-transitionsanimations)
  - [How would you center an absolutely positioned element both horizontally and vertically?](#how-would-you-center-an-absolutely-positioned-element-both-horizontally-and-vertically)
- [Responsive Design & Media Queries](#responsive-design-media-queries)
  - [What is responsive design, and what are its core techniques?](#what-is-responsive-design-and-what-are-its-core-techniques)
  - [What is the syntax of a basic media query?](#what-is-the-syntax-of-a-basic-media-query)
  - [What is the difference between mobile-first and desktop-first responsive design?](#what-is-the-difference-between-mobile-first-and-desktop-first-responsive-design)
  - [Are responsive breakpoints standardized?](#are-responsive-breakpoints-standardized)
  - [What is the difference between `min-width` and `max-width` in media queries?](#what-is-the-difference-between-min-width-and-max-width-in-media-queries)
  - [What is the difference between fluid images and using `srcset` for responsiveness?](#what-is-the-difference-between-fluid-images-and-using-srcset-for-responsiveness)
  - [What are container queries, and how do they differ from media queries?](#what-are-container-queries-and-how-do-they-differ-from-media-queries)
  - [What is the difference between `vw`/`vh` units and percentage units for responsive sizing?](#what-is-the-difference-between-vwvh-units-and-percentage-units-for-responsive-sizing)
  - [How would you make typography responsive without a huge list of media queries?](#how-would-you-make-typography-responsive-without-a-huge-list-of-media-queries)
  - [What is the difference between responsive design and adaptive design?](#what-is-the-difference-between-responsive-design-and-adaptive-design)
- [Pseudo-classes & Pseudo-elements](#pseudo-classes-pseudo-elements)
  - [What is the difference between `:hover`, `:active`, and `:focus`?](#what-is-the-difference-between-hover-active-and-focus)
  - [What do the `::before` and `::after` pseudo-elements do, and what's required for them to appear?](#what-do-the-before-and-after-pseudo-elements-do-and-whats-required-for-them-to-appear)
  - [What is the difference between `:first-child` and `:nth-child(1)`?](#what-is-the-difference-between-first-child-and-nth-child1)
  - [What is the `:checked` pseudo-class used for?](#what-is-the-checked-pseudo-class-used-for)
  - [What is the difference between `:disabled` and `[disabled]` as selectors?](#what-is-the-difference-between-disabled-and-disabled-as-selectors)
  - [What is the `::placeholder` pseudo-element used for?](#what-is-the-placeholder-pseudo-element-used-for)
  - [What is the difference between `:empty` and an element with no visible content?](#what-is-the-difference-between-empty-and-an-element-with-no-visible-content)
  - [What does the `:root` pseudo-class select, and why is it commonly used?](#what-does-the-root-pseudo-class-select-and-why-is-it-commonly-used)
  - [What is the `::selection` pseudo-element used for?](#what-is-the-selection-pseudo-element-used-for)
  - [What is the required declaration order for `:link`, `:visited`, `:hover`, and `:active`?](#what-is-the-required-declaration-order-for-link-visited-hover-and-active)
- [Animations & Transitions](#animations-transitions)
  - [What is the difference between CSS transitions and CSS animations?](#what-is-the-difference-between-css-transitions-and-css-animations)
  - [What are the key properties involved in a CSS transition?](#what-are-the-key-properties-involved-in-a-css-transition)
  - [How do you define a CSS animation with `@keyframes`?](#how-do-you-define-a-css-animation-with-keyframes)
  - [What is the difference between `transform` and changing `top`/`left`/`width`/`height` for animation?](#what-is-the-difference-between-transform-and-changing-topleftwidthheight-for-animation)
  - [What does the `animation-fill-mode` property control?](#what-does-the-animation-fill-mode-property-control)
  - [What is the difference between `animation-iteration-count: infinite` and a specific number?](#what-is-the-difference-between-animation-iteration-count-infinite-and-a-specific-number)
  - [What is the difference between `ease`, `linear`, and `cubic-bezier()` timing functions?](#what-is-the-difference-between-ease-linear-and-cubic-bezier-timing-functions)
  - [How would you pause and resume a CSS animation?](#how-would-you-pause-and-resume-a-css-animation)
  - [What is the `will-change` property, and when should you use it?](#what-is-the-will-change-property-and-when-should-you-use-it)
  - [What is the difference between animating with CSS vs. with JavaScript?](#what-is-the-difference-between-animating-with-css-vs-with-javascript)
  - [What does the `transition-delay` property do, and where is it commonly used?](#what-does-the-transition-delay-property-do-and-where-is-it-commonly-used)
- [CSS Variables, Functions & Preprocessors](#css-variables-functions-preprocessors)
  - [What are CSS custom properties (CSS variables), and how do you declare and use one?](#what-are-css-custom-properties-css-variables-and-how-do-you-declare-and-use-one)
  - [What is the difference between CSS custom properties and Sass/Less variables?](#what-is-the-difference-between-css-custom-properties-and-sassless-variables)
  - [What does the `calc()` function do, and why is it useful?](#what-does-the-calc-function-do-and-why-is-it-useful)
  - [What does the `clamp()` function do?](#what-does-the-clamp-function-do)
  - [What is a CSS preprocessor, and what problem does it solve?](#what-is-a-css-preprocessor-and-what-problem-does-it-solve)
  - [What is a mixin in Sass, and how does it differ from a function?](#what-is-a-mixin-in-sass-and-how-does-it-differ-from-a-function)
  - [What is the difference between Sass's `@import` and native CSS `@import`?](#what-is-the-difference-between-sasss-import-and-native-css-import)
  - [How does native CSS nesting compare to Sass nesting?](#how-does-native-css-nesting-compare-to-sass-nesting)
  - [What is the `env()` function used for in CSS?](#what-is-the-env-function-used-for-in-css)
  - [How would you implement dark mode using CSS custom properties?](#how-would-you-implement-dark-mode-using-css-custom-properties)
- [Advanced / Architecture](#advanced-architecture)
  - [What is BEM, and what problem does it solve?](#what-is-bem-and-what-problem-does-it-solve)
  - [What are CSS cascade layers (`@layer`), and what problem do they solve?](#what-are-css-cascade-layers-layer-and-what-problem-do-they-solve)
  - [What is the difference between utility-first CSS and traditional component-based CSS?](#what-is-the-difference-between-utility-first-css-and-traditional-component-based-css)
  - [What are CSS Modules, and what problem do they solve?](#what-are-css-modules-and-what-problem-do-they-solve)
  - [What is the difference between CSS-in-JS and traditional stylesheets?](#what-is-the-difference-between-css-in-js-and-traditional-stylesheets)
  - [Why should specificity generally trend upward through a stylesheet rather than spike unpredictably?](#why-should-specificity-generally-trend-upward-through-a-stylesheet-rather-than-spike-unpredictably)
  - [What is critical CSS, and why is it used?](#what-is-critical-css-and-why-is-it-used)
  - [What is the difference between atomic CSS and traditional semantic CSS from an architecture standpoint?](#what-is-the-difference-between-atomic-css-and-traditional-semantic-css-from-an-architecture-standpoint)
  - [What is a "specificity war," and how do teams typically prevent it?](#what-is-a-specificity-war-and-how-do-teams-typically-prevent-it)
  - [What is the difference between logical properties (like `margin-inline-start`) and physical properties (like `margin-left`)?](#what-is-the-difference-between-logical-properties-like-margin-inline-start-and-physical-properties-like-margin-left)
  - [How would you structure a large CSS codebase to keep it maintainable over time?](#how-would-you-structure-a-large-css-codebase-to-keep-it-maintainable-over-time)
- [Performance & Best Practices](#performance-best-practices)
  - [What makes some CSS selectors more expensive to match than others?](#what-makes-some-css-selectors-more-expensive-to-match-than-others)
  - [Why can animating `width`/`height`/`top`/`left` hurt performance compared to `transform`?](#why-can-animating-widthheighttopleft-hurt-performance-compared-to-transform)
  - [What is the difference between render-blocking and non-blocking CSS delivery?](#what-is-the-difference-between-render-blocking-and-non-blocking-css-delivery)
  - [How does minifying and removing unused CSS improve performance?](#how-does-minifying-and-removing-unused-css-improve-performance)
  - [What is the impact of using too many web fonts or font weights on performance?](#what-is-the-impact-of-using-too-many-web-fonts-or-font-weights-on-performance)
  - [What is the purpose of the `contain` and `content-visibility` CSS properties for performance?](#what-is-the-purpose-of-the-contain-and-content-visibility-css-properties-for-performance)
  - [Why is it generally recommended to avoid deeply nested selectors, even with preprocessors that make nesting easy?](#why-is-it-generally-recommended-to-avoid-deeply-nested-selectors-even-with-preprocessors-that-make-nesting-easy)
  - [What tools would you use to audit a page's CSS performance?](#what-tools-would-you-use-to-audit-a-pages-css-performance)
- [Behavioral / Scenario-Based Questions](#behavioral-scenario-based-questions)
  - [How would you debug a layout where an element's height isn't behaving as expected?](#how-would-you-debug-a-layout-where-an-elements-height-isnt-behaving-as-expected)
  - [How would you approach fixing specificity conflicts in a large, legacy CSS codebase?](#how-would-you-approach-fixing-specificity-conflicts-in-a-large-legacy-css-codebase)
  - [How would you build a layout that works consistently across very old and modern browsers?](#how-would-you-build-a-layout-that-works-consistently-across-very-old-and-modern-browsers)
  - [A component looks fine in isolation but breaks when placed inside another page's layout — how would you investigate?](#a-component-looks-fine-in-isolation-but-breaks-when-placed-inside-another-pages-layout-how-would-you-investigate)
  - [How would you optimize a page with a slow, CSS-heavy initial paint?](#how-would-you-optimize-a-page-with-a-slow-css-heavy-initial-paint)
  - [How would you implement a design system's spacing/color scale consistently across a codebase?](#how-would-you-implement-a-design-systems-spacingcolor-scale-consistently-across-a-codebase)
  - [How would you make sure a UI works well for users with reduced-motion preferences?](#how-would-you-make-sure-a-ui-works-well-for-users-with-reduced-motion-preferences)
  - [How would you approach reviewing a teammate's CSS pull request?](#how-would-you-approach-reviewing-a-teammates-css-pull-request)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="most-asked-tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every CSS interview. If you're short on time, start here.

<a id="what-is-css-specificity-and-how-is-it-calculated"></a>
### Q: What is CSS specificity, and how is it calculated?
**Answer:** Specificity determines which rule wins when multiple rules target the same element with conflicting declarations. It's a four-part value: inline styles, ID selectors, class/attribute/pseudo-class selectors, and element/pseudo-element selectors. Higher specificity wins regardless of source order; equal specificity falls back to whichever rule was declared last.

<a id="what-is-margin-collapsing-and-when-does-it-happen"></a>
### Q: What is margin collapsing, and when does it happen?
**Answer:** Margin collapsing happens when the vertical margins of adjacent block-level elements (or a parent and its first/last child) combine into a single margin equal to the larger of the two, instead of adding together. It only affects vertical margins in normal flow — not horizontal margins, and not elements inside `flex`/`grid` containers.

<a id="what-is-the-difference-between-display-none-and-visibility-hidden"></a>
### Q: What is the difference between `display: none` and `visibility: hidden`?
**Answer:** `display: none` removes the element entirely from the layout — it takes up no space and isn't part of the accessibility tree. `visibility: hidden` hides the element visually but it still occupies its layout space.

<a id="what-is-the-box-model-and-what-does-box-sizing-border-box-change-about-it"></a>
### Q: What is the box model, and what does `box-sizing: border-box` change about it?
**Answer:** The box model describes an element as content, padding, border, and margin, from inside out. By default (`content-box`), `width`/`height` size only the content, so padding and border add to the total rendered size. `border-box` makes `width`/`height` include padding and border, so the element's total size matches what you actually set.

<a id="what-is-the-difference-between-relative-absolute-fixed-and-sticky-positioning"></a>
### Q: What is the difference between `relative`, `absolute`, `fixed`, and `sticky` positioning?
**Answer:** `relative` positions an element relative to its own normal position without leaving flow. `absolute` removes it from flow and positions it relative to its nearest positioned ancestor. `fixed` positions relative to the viewport, staying put during scroll. `sticky` behaves like `relative` until a scroll threshold is crossed, then like `fixed` within its containing block.

<a id="what-is-the-difference-between-em-rem-and-px-units"></a>
### Q: What is the difference between `em`, `rem`, `%`, and `px` units?
**Answer:** `px` is absolute, fixed regardless of context. `em` is relative to the current element's font-size (and compounds when nested). `rem` is relative to the root `html` element's font-size, avoiding `em`'s compounding problem. `%` is relative to a parent's corresponding property.

<a id="what-is-the-difference-between-flexbox-and-grid-and-when-would-you-use-each"></a>
### Q: What is the difference between Flexbox and Grid, and when would you use each?
**Answer:** Flexbox is one-dimensional — laying items out along a single row or column — ideal for navbars or aligning items within a container. Grid is two-dimensional — laying items across rows and columns simultaneously — ideal for full page layouts or complex components. They're often combined: Grid for overall structure, Flexbox for smaller pieces within it.

<a id="why-doesnt-height-100-always-work-as-expected"></a>
### Q: Why doesn't `height: 100%` always work as expected?
**Answer:** A percentage height is calculated relative to the parent's height — but if the parent's own height is `auto` (not explicitly set), the percentage has nothing to resolve against and is effectively ignored. The whole ancestor chain needs an explicit height for percentage heights to work as expected down the tree.

<a id="what-is-the-css-cascade-and-how-does-it-decide-which-styles-apply"></a>
### Q: What is the CSS cascade, and how does it decide which styles apply?
**Answer:** The cascade decides which of multiple conflicting declarations wins, based on (in priority order): importance (`!important`), origin (author vs. browser vs. user styles), specificity, and finally source order as a tiebreaker.

<a id="what-does-important-do-and-why-is-it-generally-discouraged"></a>
### Q: What does `!important` do, and why is it generally discouraged?
**Answer:** It overrides normal specificity and cascade rules, forcing a declaration to apply regardless of what else targets the element (short of another `!important` with higher specificity). It's discouraged because it breaks the natural cascade, making styles harder to override later — usually a sign that specificity or architecture issues need fixing at the root.

<a id="what-is-the-difference-between-inline-block-and-inline-block-display-values"></a>
### Q: What is the difference between `inline`, `block`, and `inline-block` display values?
**Answer:** `block` elements take the full available width and start on a new line. `inline` elements flow within text, only as wide as their content, and ignore `width`/`height`/vertical margin. `inline-block` sits inline like text but respects `width`, `height`, and margin/padding like a block element.

<a id="how-does-z-index-work-and-why-doesnt-it-always-behave-as-expected"></a>
### Q: How does `z-index` work, and why doesn't it always behave as expected?
**Answer:** `z-index` controls stacking order, but only affects positioned elements (`position` other than `static`), and only within the same stacking context. Properties like `opacity < 1`, `transform`, or `filter` create a new stacking context — so a high `z-index` inside one stacking context can still render behind a lower `z-index` element in a different, higher-level context.

<a id="what-is-the-difference-between-hover-and-focus-and-why-do-both-matter"></a>
### Q: What is the difference between `:hover` and `:focus`, and why do both matter?
**Answer:** `:hover` applies while the mouse pointer is over an element — irrelevant for touch or keyboard-only users. `:focus` applies when an element has keyboard focus — critical for keyboard and assistive-technology users. Good UX styles both rather than relying on `:hover` alone.

<a id="what-is-a-css-reset-or-normalize-and-why-use-one"></a>
### Q: What is a CSS reset or normalize, and why use one?
**Answer:** Browsers apply different default styles (margins, font sizes, list styles), causing inconsistent starting points. A "reset" strips almost all default styling to a blank slate; a "normalize" instead makes defaults consistent across browsers while preserving useful baseline styling. Either approach reduces cross-browser surprises.

<a id="what-is-the-difference-between-min-widthmax-width-and-width"></a>
### Q: What is the difference between `min-width`/`max-width` and `width`?
**Answer:** `width` sets a fixed target size. `min-width` sets a floor the element won't shrink below; `max-width` sets a ceiling it won't grow beyond. Combining `width: 100%` with a `max-width` is a very common responsive pattern — fluid up to a cap.

<a id="what-is-a-stacking-context-and-what-commonly-creates-one-by-surprise"></a>
### Q: What is a stacking context, and what commonly creates one by surprise?
**Answer:** A stacking context is an isolated "layer" for `z-index` comparisons — values are only compared within the same context. Beyond `position` + `z-index`, properties like `opacity` less than 1, `transform`, `filter`, and `will-change` also silently create new stacking contexts, a frequent source of "why isn't my `z-index` working" bugs.

---

<a id="css-basics"></a>
## CSS Basics

<a id="what-is-css-and-what-problem-does-it-solve"></a>
### Q: What is CSS, and what problem does it solve?
**Answer:** CSS (Cascading Style Sheets) controls the visual presentation of HTML — colors, layout, typography, spacing — separating content/structure from presentation, which makes both easier to maintain and lets one stylesheet consistently style many pages.

<a id="what-are-the-three-ways-to-add-css-to-an-html-page"></a>
### Q: What are the three ways to add CSS to an HTML page?
**Answer:** Inline (a `style` attribute directly on an element), internal (a `<style>` block in `<head>`), and external (a separate `.css` file linked via `<link rel="stylesheet">`). External stylesheets are generally preferred for maintainability and caching.

<a id="what-is-the-basic-syntax-of-a-css-rule"></a>
### Q: What is the basic syntax of a CSS rule?
**Answer:** A selector followed by a declaration block in curly braces containing one or more `property: value;` pairs.

**Example:**
```css
p {
  color: blue;
  font-size: 16px;
}
```

<a id="what-is-the-difference-between-a-class-selector-and-an-id-selector"></a>
### Q: What is the difference between a class selector and an id selector?
**Answer:** A class selector (`.classname`) can apply to multiple elements and be reused. An id selector (`#idname`) should be unique per page, targeting exactly one element. IDs also carry much higher specificity than classes, which can make overriding their styles harder later.

<a id="how-do-you-write-css-comments"></a>
### Q: How do you write CSS comments?
**Answer:** `/* comment text */` — CSS has no single-line comment syntax like `//`; everything between `/*` and `*/` is ignored by the browser.

<a id="what-is-the-difference-between-shorthand-and-longhand-css-properties"></a>
### Q: What is the difference between shorthand and longhand CSS properties?
**Answer:** Shorthand properties combine several related longhand properties into one declaration (e.g. `margin: 10px 20px;` sets top/bottom and left/right at once). Longhand properties set each aspect individually (`margin-top`, `margin-right`, etc.) — more verbose, but more explicit and easier to override selectively.

<a id="what-is-the-difference-between-absolute-and-relative-css-units"></a>
### Q: What is the difference between absolute and relative CSS units?
**Answer:** Absolute units (`px`, `cm`, `in`) represent a fixed size regardless of context. Relative units (`em`, `rem`, `%`, `vw`, `vh`) scale based on another value — a parent's size, the root font-size, or the viewport — making them more useful for responsive, flexible designs.

<a id="what-is-the-difference-between-color-background-color-and-border-color"></a>
### Q: What is the difference between `color`, `background-color`, and `border-color`?
**Answer:** `color` sets the text (foreground) color of an element. `background-color` sets the fill color behind the content/padding area. `border-color` sets the border's color, independent of the other two.

<a id="how-do-you-apply-a-css-rule-to-multiple-selectors-at-once"></a>
### Q: How do you apply a CSS rule to multiple selectors at once?
**Answer:** Separate selectors with a comma — each gets the same declaration block applied independently.

**Example:**
```css
h1, h2, h3 {
  font-family: sans-serif;
}
```

<a id="where-is-important-placed-in-a-declaration"></a>
### Q: Where is `!important` placed in a declaration?
**Answer:** Appended directly after a property's value, before the semicolon — `color: red !important;`. It overrides normal cascade/specificity rules for that specific declaration.

<a id="what-is-the-difference-between-content-box-and-border-box-in-box-sizing"></a>
### Q: What is the difference between `content-box` and `border-box` in `box-sizing`?
**Answer:** `content-box` (the default) sizes `width`/`height` to the content only, so padding/border add to the total rendered size. `border-box` includes padding and border within that size, so the element's total rendered size matches what you set — much easier to reason about.

<a id="what-is-the-difference-between-inherit-initial-and-unset-as-css-values"></a>
### Q: What is the difference between `inherit`, `initial`, and `unset` as CSS values?
**Answer:** `inherit` forces a property to take its parent's computed value, even for properties that don't inherit by default. `initial` resets a property to its spec-defined default. `unset` acts like `inherit` for properties that naturally inherit (like `color`), or like `initial` for ones that don't (like `margin`).

---

<a id="selectors-specificity"></a>
## Selectors & Specificity

<a id="what-is-the-difference-between-a-descendant-selector-and-a-child-selector"></a>
### Q: What is the difference between a descendant selector and a child selector?
**Answer:** A descendant selector (`div p`, space-separated) matches a `p` anywhere inside a `div`, no matter how deeply nested. A child selector (`div > p`) matches only a `p` that is a **direct** child of the `div`.

<a id="what-is-the-difference-between-the-adjacent-sibling-and-general-sibling-combinators"></a>
### Q: What is the difference between the adjacent sibling (+) and general sibling (~) combinators?
**Answer:** `A + B` selects a `B` immediately preceded by an `A` sibling (the very next element). `A ~ B` selects any `B` sibling that comes after `A`, not necessarily immediately adjacent, as long as they share the same parent.

<a id="what-are-attribute-selectors-and-how-do-you-use-them"></a>
### Q: What are attribute selectors, and how do you use them?
**Answer:** They select elements based on the presence or value of an HTML attribute, e.g. `[type="text"]`, `[href^="https"]` (starts with), `[href$=".pdf"]` (ends with), `[class*="btn"]` (contains).

**Example:**
```css
input[type="checkbox"] {
  margin-right: 8px;
}
```

<a id="what-is-the-universal-selector-and-when-is-it-used"></a>
### Q: What is the universal selector, and when is it used?
**Answer:** `*` matches every element on the page. Commonly used in CSS resets, e.g. `* { margin: 0; padding: 0; box-sizing: border-box; }`, though broad use can hurt performance slightly and should be applied thoughtfully.

<a id="what-is-the-difference-between-a-pseudo-class-and-a-pseudo-element"></a>
### Q: What is the difference between a pseudo-class and a pseudo-element?
**Answer:** A pseudo-class (single colon, e.g. `:hover`, `:first-child`) selects an element based on a state or position it's already in. A pseudo-element (double colon, e.g. `::before`, `::first-line`) targets a specific sub-part of an element, or generates new content that isn't an actual element in the DOM.

<a id="how-is-specificity-calculated-step-by-step"></a>
### Q: How is specificity calculated, step by step?
**Answer:** Specificity is a 4-part tuple: inline styles, IDs, classes/attributes/pseudo-classes, and elements/pseudo-elements. Count how many of each appear in a selector and compare left to right — inline beats any number of IDs, an ID beats any number of classes, a class beats any number of elements. `!important` overrides specificity entirely.

<a id="what-is-the-difference-between-nth-child-and-nth-of-type"></a>
### Q: What is the difference between `:nth-child()` and `:nth-of-type()`?
**Answer:** `:nth-child(n)` selects based on an element's position among ALL sibling elements of any type. `:nth-of-type(n)` selects based on position among siblings of the SAME element type only — the counts can differ when a container has mixed element types.

<a id="what-does-the-not-pseudo-class-do"></a>
### Q: What does the `:not()` pseudo-class do?
**Answer:** It excludes elements matching the given selector from an otherwise-matching set.

**Example:**
```css
li:not(.active) {
  opacity: 0.5;
}
```

<a id="what-is-the-difference-between-first-child-and-first-of-type"></a>
### Q: What is the difference between `:first-child` and `:first-of-type`?
**Answer:** `:first-child` matches an element only if it's the very first child of its parent, regardless of type. `:first-of-type` matches if it's the first sibling of its specific element type, even if other, different elements come before it.

<a id="does-selector-order-or-structure-affect-matching-performance"></a>
### Q: Does selector order or structure affect matching performance?
**Answer:** Browsers match selectors right to left, so a very generic rightmost selector combined with a long ancestor chain can be more expensive across a large DOM. In practice modern browsers are highly optimized and this rarely matters for typical sites, but avoiding excessively long, overly generic selector chains is still good practice.

<a id="what-is-the-is-and-where-selector-and-what-problem-does-it-solve"></a>
### Q: What is the `:is()` (and `:where()`) selector, and what problem does it solve?
**Answer:** `:is(selector-list)` groups multiple selectors sharing the same following selector into one compact rule, e.g. `:is(header, footer) a` instead of `header a, footer a`. `:where()` behaves the same but always has zero specificity, useful for easily-overridable base styles.

<a id="what-is-the-difference-between-class1class2-and-class1-class2-as-selectors"></a>
### Q: What is the difference between `.class1.class2` and `.class1 .class2` as selectors?
**Answer:** `.class1.class2` (no space) selects a single element that has BOTH classes applied. `.class1 .class2` (with a space) selects a descendant element with `class2` nested inside an ancestor with `class1` — two different elements.

---

<a id="box-model-layout"></a>
## Box Model & Layout

<a id="what-are-the-four-parts-of-the-css-box-model-from-inside-out"></a>
### Q: What are the four parts of the CSS box model, from inside out?
**Answer:** Content (the actual text/image/etc.), padding (space between content and border), border (the line around padding), and margin (space outside the border, between this element and others).

<a id="what-is-the-difference-between-margin-and-padding"></a>
### Q: What is the difference between margin and padding?
**Answer:** Padding is space INSIDE an element's border — part of its clickable/background area. Margin is space OUTSIDE the border — it creates separation from neighboring elements and isn't part of the element's own background.

<a id="what-causes-margin-collapsing-and-how-do-you-prevent-it"></a>
### Q: What causes margin collapsing, and how do you prevent it?
**Answer:** Adjacent vertical margins between block-level siblings (or a parent/first-child, parent/last-child pair) collapse into one, taking the larger value. Prevent it by adding padding or a border to the parent, using `display: flex`/`grid` on the parent (collapsing doesn't happen there), or `overflow: auto`/`hidden` to establish a new block formatting context.

<a id="what-is-a-block-formatting-context-bfc-and-why-does-it-matter"></a>
### Q: What is a Block Formatting Context (BFC), and why does it matter?
**Answer:** A BFC is an isolated layout region where floats and margins are contained and don't interact with content outside it. Ways to trigger one: `overflow: hidden`/`auto`, `display: flow-root`, `float`, or `position: absolute`/`fixed`. Frequently used to contain floated children or prevent margin collapsing.

<a id="what-is-the-difference-between-overflow-visible-hidden-scroll-and-auto"></a>
### Q: What is the difference between `overflow: visible`, `hidden`, `scroll`, and `auto`?
**Answer:** `visible` (default) lets content spill outside the box unclipped. `hidden` clips overflowing content entirely, no scrollbar. `scroll` always shows scrollbars, even if content fits. `auto` shows scrollbars only when content actually overflows.

<a id="how-do-you-horizontally-and-vertically-center-a-block-element"></a>
### Q: How do you horizontally and vertically center a block element?
**Answer:** For a fixed-width block, `margin: 0 auto;` centers it horizontally. For full centering on any parent, make the parent a flex container: `display: flex; justify-content: center; align-items: center;`.

<a id="what-is-the-difference-between-width-100-and-width-100vw"></a>
### Q: What is the difference between `width: 100%` and `width: 100vw`?
**Answer:** `100%` is relative to the parent element's width. `100vw` is relative to the full viewport width, which can cause horizontal overflow if the page has a vertical scrollbar, since `vw` includes the scrollbar's width in some browsers while a parent's actual rendered width doesn't.

<a id="what-are-floats-and-what-were-they-historically-used-for"></a>
### Q: What are floats, and what were they historically used for?
**Answer:** `float: left`/`right` takes an element out of normal flow and pushes it to one side, letting inline content wrap around it — originally used for text-wrapping around images, later misused for full page layout before Flexbox/Grid existed. Modern layout should use Flexbox or Grid instead.

<a id="what-is-the-clearfix-technique-and-why-was-it-needed"></a>
### Q: What is the "clearfix" technique, and why was it needed?
**Answer:** A floated element doesn't contribute to its parent's height, so a parent containing only floated children can visually collapse to zero height. The clearfix technique (`.clearfix::after { content: ""; display: table; clear: both; }`) forces the parent to properly contain its floated children.

<a id="what-is-the-difference-between-visibility-collapse-and-display-none-for-table-rows"></a>
### Q: What is the difference between `visibility: collapse` and `display: none` for table rows?
**Answer:** `visibility: collapse` on a table row removes it visually and reclaims its space specifically within table layout — but the row still exists in the DOM/accessibility tree, unlike `display: none`, which removes it from both layout and accessibility entirely.

---

<a id="flexbox"></a>
## Flexbox

<a id="what-is-flexbox-and-what-problem-does-it-solve"></a>
### Q: What is Flexbox, and what problem does it solve?
**Answer:** Flexbox (`display: flex`) is a one-dimensional layout model for distributing space and aligning items along a single row or column, solving problems that used to require hacky float/table-based layouts — like vertical centering, equal-height columns, and flexible item sizing.

<a id="what-is-the-difference-between-the-main-axis-and-the-cross-axis-in-flexbox"></a>
### Q: What is the difference between the main axis and the cross axis in Flexbox?
**Answer:** The main axis runs in the direction set by `flex-direction` (row by default) — `justify-content` aligns items along it. The cross axis runs perpendicular — `align-items` aligns items along it.

<a id="what-do-flex-grow-flex-shrink-and-flex-basis-each-control"></a>
### Q: What do `flex-grow`, `flex-shrink`, and `flex-basis` each control?
**Answer:** `flex-grow` determines how much an item expands into extra available space, relative to other items' grow values. `flex-shrink` determines how much an item shrinks when space is tight, relative to others. `flex-basis` sets an item's initial main-axis size before growing/shrinking is applied.

<a id="what-does-justify-content-control-and-what-are-its-common-values"></a>
### Q: What does `justify-content` control, and what are its common values?
**Answer:** It aligns flex items along the main axis. Common values: `flex-start`, `flex-end`, `center`, `space-between` (items spread with no space at the edges), `space-around` (equal space around each item), `space-evenly` (fully equal spacing including edges).

<a id="what-does-align-items-control-versus-align-content"></a>
### Q: What does `align-items` control, versus `align-content`?
**Answer:** `align-items` aligns items along the cross axis within a single line. `align-content` aligns entire lines of items along the cross axis when there's extra space and the container has multiple flex lines (`flex-wrap: wrap`) — it has no effect with only one line.

<a id="what-does-align-self-do-and-how-does-it-differ-from-align-items"></a>
### Q: What does `align-self` do, and how does it differ from `align-items`?
**Answer:** `align-items` sets cross-axis alignment for ALL flex items at the container level. `align-self`, set on an individual item, overrides that container-level alignment for just that one item.

<a id="what-is-the-shorthand-flex-property-and-what-does-flex-1-mean"></a>
### Q: What is the shorthand `flex` property, and what does `flex: 1` mean?
**Answer:** `flex` is shorthand for `flex-grow flex-shrink flex-basis`. `flex: 1` expands to `flex: 1 1 0%` — the item can grow and shrink equally with other `flex: 1` siblings, ignoring content size as a starting basis, effectively splitting available space evenly.

<a id="what-does-flex-wrap-do-and-whats-the-difference-between-wrap-and-nowrap"></a>
### Q: What does `flex-wrap` do, and what's the difference between `wrap` and `nowrap`?
**Answer:** `flex-wrap` controls whether items are forced onto a single line or allowed to wrap onto multiple lines. `nowrap` (default) squeezes all items onto one line even if they overflow or shrink awkwardly. `wrap` lets items flow onto new lines when they don't fit.

<a id="how-do-you-reverse-the-order-of-flex-items-without-changing-the-html"></a>
### Q: How do you reverse the order of flex items without changing the HTML?
**Answer:** Set `flex-direction: row-reverse` or `column-reverse` on the container — though this can create accessibility mismatches between visual and DOM/tab order, so it should be used carefully.

<a id="how-would-you-build-a-classic-sticky-footer-layout-using-flexbox"></a>
### Q: How would you build a classic "sticky footer" layout using Flexbox?
**Answer:** Make the page's outer wrapper `display: flex; flex-direction: column; min-height: 100vh;`, and give the main content area `flex: 1` so it expands to fill leftover vertical space, pushing the footer to the bottom of the viewport even on short pages.

---

<a id="grid"></a>
## Grid

<a id="what-is-css-grid-and-how-does-it-differ-from-flexbox"></a>
### Q: What is CSS Grid, and how does it differ from Flexbox?
**Answer:** CSS Grid (`display: grid`) is a two-dimensional layout system, letting you define both rows and columns simultaneously and place items precisely within that grid. Flexbox is one-dimensional — Grid is generally better for overall page layout, Flexbox for smaller, linear component layouts.

<a id="how-do-you-define-columns-and-rows-in-a-grid-container"></a>
### Q: How do you define columns and rows in a Grid container?
**Answer:** Using `grid-template-columns` and `grid-template-rows`, specifying a size for each track.

**Example:**
```css
.container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  grid-template-rows: auto 1fr auto;
}
```

<a id="what-is-the-fr-unit-in-grid-and-how-does-it-work"></a>
### Q: What is the `fr` unit in Grid, and how does it work?
**Answer:** `fr` represents a fraction of the remaining available space in the grid container, after fixed-size tracks are accounted for. `grid-template-columns: 1fr 2fr` splits leftover space into 3 parts, giving the second column twice the space of the first.

<a id="what-is-the-difference-between-grid-template-areas-and-manually-placing-items-with-line-numbers"></a>
### Q: What is the difference between `grid-template-areas` and manually placing items with line numbers?
**Answer:** `grid-template-areas` lets you name grid regions in a visual, ASCII-art-like layout and assign items to named areas — often more readable for complex layouts. Placing items with `grid-column`/`grid-row` line numbers gives precise numeric control, more flexible for irregular or dynamic layouts.

**Example:**
```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer";
}
.sidebar { grid-area: sidebar; }
```

<a id="what-does-repeat-do-in-a-grid-template-columns-declaration"></a>
### Q: What does `repeat()` do in a `grid-template-columns` declaration?
**Answer:** It's shorthand for repeating a track pattern a number of times — `repeat(3, 1fr)` is equivalent to `1fr 1fr 1fr` — useful especially combined with `auto-fill`/`auto-fit` for responsive grids that adjust column count automatically.

<a id="what-is-the-difference-between-auto-fill-and-auto-fit-in-repeat"></a>
### Q: What is the difference between `auto-fill` and `auto-fit` in `repeat()`?
**Answer:** Both automatically create as many tracks as fit the container. `auto-fill` keeps empty tracks as placeholders if there isn't enough content, potentially leaving gaps. `auto-fit` collapses empty tracks to zero width, letting existing items stretch to fill the leftover space instead.

<a id="what-do-grid-column-and-grid-row-shorthand-properties-do"></a>
### Q: What do `grid-column` and `grid-row` shorthand properties do?
**Answer:** They place a grid item by specifying start and end grid lines — `grid-column: 1 / 3` spans the item from line 1 to line 3 (across two columns). `span` can also be used: `grid-column: span 2` spans two columns from the item's placement.

<a id="what-is-the-gap-property-and-row-gapcolumn-gap-in-gridflexbox"></a>
### Q: What is the `gap` property (and `row-gap`/`column-gap`) in Grid/Flexbox?
**Answer:** `gap` sets spacing between grid or flex items directly, without needing extra margin hacks that could cause uneven spacing at the edges. `row-gap` and `column-gap` control vertical and horizontal spacing independently.

<a id="how-would-you-build-a-responsive-grid-without-using-media-queries"></a>
### Q: How would you build a responsive grid without using media queries?
**Answer:** Combine `repeat(auto-fit, minmax(200px, 1fr))` in `grid-template-columns` — each column is at least 200px but grows to fill available space, and the number of columns adjusts automatically as the container width changes, without an explicit breakpoint.

<a id="what-is-the-difference-between-implicit-and-explicit-grid-tracks"></a>
### Q: What is the difference between implicit and explicit grid tracks?
**Answer:** Explicit tracks are the ones you define directly with `grid-template-columns`/`grid-template-rows`. Implicit tracks are automatically created when content is placed outside those explicit tracks (e.g. more items than defined columns/rows) — sized by `grid-auto-columns`/`grid-auto-rows` if specified, or their default `auto` size otherwise.

---

<a id="positioning-display"></a>
## Positioning & Display

<a id="what-are-the-possible-values-of-the-position-property-and-what-does-each-do"></a>
### Q: What are the possible values of the `position` property, and what does each do?
**Answer:** `static` (default, normal flow, offset properties have no effect), `relative` (offset from its own normal position without leaving flow), `absolute` (removed from flow, positioned relative to the nearest positioned ancestor), `fixed` (relative to the viewport, ignoring scroll), `sticky` (relative until a scroll threshold, then fixed within its container).

<a id="what-is-a-positioned-ancestor-and-why-does-it-matter-for-absolute-positioning"></a>
### Q: What is a "positioned ancestor," and why does it matter for absolute positioning?
**Answer:** A positioned ancestor is any ancestor with a `position` value other than `static`. An absolutely positioned element is placed relative to its nearest positioned ancestor — if none exists, it falls back to the initial containing block, which is why adding `position: relative` to a parent (even with no offsets) is a common way to "contain" an absolutely positioned child.

<a id="what-is-the-difference-between-display-none-and-opacity-0"></a>
### Q: What is the difference between `display: none` and `opacity: 0`?
**Answer:** `display: none` removes the element from layout entirely — no space, not interactive, not in the accessibility tree. `opacity: 0` makes it fully transparent but it still occupies its space and remains interactive (clickable, focusable) and present for assistive technology unless separately hidden.

<a id="how-does-position-sticky-actually-work-and-whats-a-common-gotcha"></a>
### Q: How does `position: sticky` actually work, and what's a common gotcha?
**Answer:** A sticky element behaves like `relative` until the viewport scrolls past a threshold (via `top`, `bottom`, etc.), then "sticks" like `fixed`, but only within its containing block — once the parent scrolls out of view, the sticky element scrolls away with it. Common gotcha: it silently fails to stick if any ancestor has `overflow: hidden`/`auto`/`scroll` set.

<a id="what-is-the-difference-between-display-inline-block-and-float-for-laying-out-elements-side-by-side"></a>
### Q: What is the difference between `display: inline-block` and `float` for laying out elements side by side?
**Answer:** `inline-block` keeps elements in normal flow, respecting width/height/margins like block elements, while being subject to whitespace gaps between inline elements in the HTML source. `float` removes elements from normal flow entirely, requiring clearfix techniques. Flexbox has largely replaced both approaches today.

<a id="what-is-a-stacking-context-and-what-creates-one"></a>
### Q: What is a stacking context, and what creates one?
**Answer:** A conceptual "layer" for `z-index` comparisons — values are only compared directly within the same stacking context. New stacking contexts are created by any positioned element with a non-`auto` z-index, `opacity` less than 1, `transform`, `filter`, `will-change`, or the root element itself, among others.

<a id="what-is-the-difference-between-toprightbottomleft-on-a-static-vs-relativeabsolute-element"></a>
### Q: What is the difference between `top`/`right`/`bottom`/`left` on a `static` vs. `relative`/`absolute` element?
**Answer:** On `static` (the default), these offsets have no effect at all. On `relative`, they shift the element from its normal position without affecting other elements' layout. On `absolute`/`fixed`, they determine the element's actual position relative to its positioning context.

<a id="what-does-display-contents-do"></a>
### Q: What does `display: contents` do?
**Answer:** It makes an element's own box disappear from rendering (no visible box, background, or border), while its children render as if they were direct children of the element's own parent — useful for wrapper elements needed for markup/JS that shouldn't affect layout.

<a id="what-is-the-difference-between-visibility-hidden-and-display-none-in-terms-of-transitionsanimations"></a>
### Q: What is the difference between `visibility: hidden` and `display: none` in terms of transitions/animations?
**Answer:** `display: none` can't be transitioned smoothly — an element abruptly appears/disappears. `visibility: hidden` (and `opacity`) CAN be transitioned, allowing fade in/out effects, though `visibility` alone only supports a hard flip at 50% unless combined with `opacity` for a real fade.

<a id="how-would-you-center-an-absolutely-positioned-element-both-horizontally-and-vertically"></a>
### Q: How would you center an absolutely positioned element both horizontally and vertically?
**Answer:** A classic technique: `position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%);` — positioning the element's top-left corner at the center point, then shifting it back by half its own width/height using `transform`, which is based on the element's own size (unlike percentage offsets).

---

<a id="responsive-design-media-queries"></a>
## Responsive Design & Media Queries

<a id="what-is-responsive-design-and-what-are-its-core-techniques"></a>
### Q: What is responsive design, and what are its core techniques?
**Answer:** Responsive design means a layout adapts to different screen sizes and devices using a single codebase. Core techniques: fluid/percentage-based sizing, flexible images, media queries for breakpoint-specific styles, and a correctly configured viewport meta tag.

<a id="what-is-the-syntax-of-a-basic-media-query"></a>
### Q: What is the syntax of a basic media query?
**Answer:** `@media` followed by a condition, wrapping the CSS rules that should apply only when that condition is true.

**Example:**
```css
@media (max-width: 768px) {
  .sidebar { display: none; }
}
```

<a id="what-is-the-difference-between-mobile-first-and-desktop-first-responsive-design"></a>
### Q: What is the difference between mobile-first and desktop-first responsive design?
**Answer:** Mobile-first writes base styles for small screens, then uses `min-width` media queries to progressively add complexity for larger screens. Desktop-first writes base styles for large screens, then uses `max-width` queries to simplify for smaller ones. Mobile-first is generally recommended since it tends to produce leaner CSS.

<a id="are-responsive-breakpoints-standardized"></a>
### Q: Are responsive breakpoints standardized?
**Answer:** No — breakpoints should ideally be based on where YOUR content/design actually breaks, not arbitrary device widths. Common conventional ranges are roughly: mobile (under 576px), tablet (576–768px), small desktop (768–992px), and large desktop (992px+).

<a id="what-is-the-difference-between-min-width-and-max-width-in-media-queries"></a>
### Q: What is the difference between `min-width` and `max-width` in media queries?
**Answer:** `(min-width: 768px)` matches when the viewport is AT LEAST 768px wide (mobile-first, "apply from this size up"). `(max-width: 768px)` matches when the viewport is AT MOST 768px wide (desktop-first, "apply up to this size").

<a id="what-is-the-difference-between-fluid-images-and-using-srcset-for-responsiveness"></a>
### Q: What is the difference between fluid images and using `srcset` for responsiveness?
**Answer:** `img { max-width: 100%; height: auto; }` is a CSS technique that scales an image down to fit its container, but the browser still downloads the full-resolution file regardless of display size. `srcset` (an HTML attribute) lets the browser choose and download an appropriately-sized file for the actual rendered size/density, saving bandwidth — the two are often used together.

<a id="what-are-container-queries-and-how-do-they-differ-from-media-queries"></a>
### Q: What are container queries, and how do they differ from media queries?
**Answer:** Media queries respond to the viewport's size. Container queries (`@container`) let a component's styles respond to the size of its own containing element instead — useful for components that need to adapt based on where they're placed, regardless of overall viewport size.

**Example:**
```css
.card-container { container-type: inline-size; }
@container (min-width: 400px) {
  .card { flex-direction: row; }
}
```

<a id="what-is-the-difference-between-vwvh-units-and-percentage-units-for-responsive-sizing"></a>
### Q: What is the difference between `vw`/`vh` units and percentage units for responsive sizing?
**Answer:** `vw`/`vh` are always relative to the viewport's width/height, regardless of an element's parent. `%` is relative to the element's parent's corresponding dimension. `vw`/`vh` suit truly viewport-relative sizing (a full-bleed hero); `%` suits sizing relative to a local container.

<a id="how-would-you-make-typography-responsive-without-a-huge-list-of-media-queries"></a>
### Q: How would you make typography responsive without a huge list of media queries?
**Answer:** Use `clamp(min, preferred, max)` with a viewport-relative unit in the preferred value, e.g. `font-size: clamp(1rem, 2vw + 0.5rem, 2rem);` — the size scales fluidly with viewport width between the defined minimum and maximum, without discrete breakpoints.

<a id="what-is-the-difference-between-responsive-design-and-adaptive-design"></a>
### Q: What is the difference between responsive design and adaptive design?
**Answer:** Responsive design uses fluid, flexible layouts that continuously adapt across the full range of screen sizes. Adaptive design instead serves a small number of fixed, distinct layouts targeted at specific breakpoints, switching between them rather than fluidly scaling.

---

<a id="pseudo-classes-pseudo-elements"></a>
## Pseudo-classes & Pseudo-elements

<a id="what-is-the-difference-between-hover-active-and-focus"></a>
### Q: What is the difference between `:hover`, `:active`, and `:focus`?
**Answer:** `:hover` applies while the pointer is over the element. `:active` applies during the moment it's being clicked (mouse button down). `:focus` applies when the element currently has keyboard/programmatic focus, regardless of pointer device.

<a id="what-do-the-before-and-after-pseudo-elements-do-and-whats-required-for-them-to-appear"></a>
### Q: What do the `::before` and `::after` pseudo-elements do, and what's required for them to appear?
**Answer:** They insert generated content immediately before or after an element's actual content, without adding anything to the HTML markup. They require a `content` property (even `content: "";` for an empty visual element) — without it, they won't render at all.

**Example:**
```css
.tooltip::after {
  content: "";
  display: block;
}
```

<a id="what-is-the-difference-between-first-child-and-nth-child1"></a>
### Q: What is the difference between `:first-child` and `:nth-child(1)`?
**Answer:** They select the same element in most cases. `:nth-child(1)` is more flexible since `nth-child()` also supports formulas (`2n`, `odd`, `3n+1`), while `:first-child` is just a fixed shorthand for that one case.

<a id="what-is-the-checked-pseudo-class-used-for"></a>
### Q: What is the `:checked` pseudo-class used for?
**Answer:** It matches checkboxes, radio buttons, or `<option>` elements currently checked/selected — commonly used with the "checkbox hack" to build pure-CSS toggles (like a mobile menu or accordion) by styling a sibling element differently based on a hidden checkbox's checked state.

<a id="what-is-the-difference-between-disabled-and-disabled-as-selectors"></a>
### Q: What is the difference between `:disabled` and `[disabled]` as selectors?
**Answer:** `:disabled` is a proper pseudo-class matching any element in a disabled state per its semantic meaning. `[disabled]` is an attribute selector matching elements with a literal `disabled` attribute in the HTML. They usually select the same elements, but `:disabled` is considered more semantically correct.

<a id="what-is-the-placeholder-pseudo-element-used-for"></a>
### Q: What is the `::placeholder` pseudo-element used for?
**Answer:** It styles the placeholder text inside an empty `<input>` or `<textarea>` before the user types, letting you change its color, font-style, or opacity independent of the actual typed text's styling.

<a id="what-is-the-difference-between-empty-and-an-element-with-no-visible-content"></a>
### Q: What is the difference between `:empty` and an element with no visible content?
**Answer:** `:empty` matches an element with absolutely no children at all — not even whitespace text nodes. An element containing only whitespace (like a stray space between tags) technically has a text node child and won't match `:empty`, which often surprises developers.

<a id="what-does-the-root-pseudo-class-select-and-why-is-it-commonly-used"></a>
### Q: What does the `:root` pseudo-class select, and why is it commonly used?
**Answer:** `:root` matches the document's root element (`<html>`), functionally similar to the `html` selector but with higher specificity. It's the conventional place to define global CSS custom properties, since they cascade down to the entire document from there.

<a id="what-is-the-selection-pseudo-element-used-for"></a>
### Q: What is the `::selection` pseudo-element used for?
**Answer:** It styles the portion of text a user has currently highlighted with their cursor, commonly used to customize the selection's background and text color to match a site's branding instead of the browser default.

<a id="what-is-the-required-declaration-order-for-link-visited-hover-and-active"></a>
### Q: What is the required declaration order for `:link`, `:visited`, `:hover`, and `:active`?
**Answer:** They should be declared in that order — `:link`, `:visited`, `:hover`, `:active` (mnemonic "LoVe HAte") — because later rules of equal specificity override earlier ones. Declaring them out of order can cause `:hover`/`:active` styles to be silently overridden by `:link`/`:visited` due to source order.

---

<a id="animations-transitions"></a>
## Animations & Transitions

<a id="what-is-the-difference-between-css-transitions-and-css-animations"></a>
### Q: What is the difference between CSS transitions and CSS animations?
**Answer:** Transitions smoothly interpolate a property between two states (a start and end), typically triggered by a state change like `:hover` — they need a trigger and run once between two defined states. Animations (`@keyframes`) can define multiple intermediate steps, run automatically without a trigger, loop indefinitely, and offer far more control over timing at each stage.

<a id="what-are-the-key-properties-involved-in-a-css-transition"></a>
### Q: What are the key properties involved in a CSS transition?
**Answer:** `transition-property` (which property to animate), `transition-duration` (how long it takes), `transition-timing-function` (the easing curve, e.g. `ease`, `linear`, `cubic-bezier()`), and `transition-delay` (how long to wait before starting) — often combined into the `transition` shorthand.

**Example:**
```css
.box {
  transition: transform 0.3s ease, opacity 0.3s ease;
}
```

<a id="how-do-you-define-a-css-animation-with-keyframes"></a>
### Q: How do you define a CSS animation with `@keyframes`?
**Answer:** Define named keyframes describing property values at various points (percentages, or `from`/`to`), then reference that name with the `animation` property on an element.

**Example:**
```css
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
.box {
  animation: fadeIn 1s ease-in;
}
```

<a id="what-is-the-difference-between-transform-and-changing-topleftwidthheight-for-animation"></a>
### Q: What is the difference between `transform` and changing `top`/`left`/`width`/`height` for animation?
**Answer:** `transform` (translate, scale, rotate) and `opacity` can typically be animated on the GPU's compositor thread, without triggering layout recalculation of surrounding content — much better performance. Animating `top`/`left`/`width`/`height` directly usually triggers layout (reflow) on every frame, significantly more expensive.

<a id="what-does-the-animation-fill-mode-property-control"></a>
### Q: What does the `animation-fill-mode` property control?
**Answer:** It controls what styles apply before the animation starts and/or after it ends. `forwards` keeps the last keyframe's styles after finishing; `backwards` applies the first keyframe's styles during any `animation-delay`; `both` applies both behaviors.

<a id="what-is-the-difference-between-animation-iteration-count-infinite-and-a-specific-number"></a>
### Q: What is the difference between `animation-iteration-count: infinite` and a specific number?
**Answer:** `infinite` loops the animation forever until removed or the element is hidden/unmounted. A specific number (e.g. `3`) runs it that many times, then stops and — depending on `fill-mode` — either reverts to the original styles or holds on the final keyframe's values.

<a id="what-is-the-difference-between-ease-linear-and-cubic-bezier-timing-functions"></a>
### Q: What is the difference between `ease`, `linear`, and `cubic-bezier()` timing functions?
**Answer:** `linear` moves at a constant rate throughout. `ease` (the default) starts slowly, speeds up, then slows down near the end, feeling more natural. `cubic-bezier(x1, y1, x2, y2)` lets you define a fully custom easing curve for precise control.

<a id="how-would-you-pause-and-resume-a-css-animation"></a>
### Q: How would you pause and resume a CSS animation?
**Answer:** Set `animation-play-state: paused;` to freeze it on the current frame, and `animation-play-state: running;` to resume — commonly toggled via JavaScript or a `:hover` state.

<a id="what-is-the-will-change-property-and-when-should-you-use-it"></a>
### Q: What is the `will-change` property, and when should you use it?
**Answer:** `will-change` hints to the browser that a property is about to change soon (e.g. `will-change: transform;`), letting it proactively optimize rendering ahead of time. Use it sparingly, only on elements that will genuinely animate soon — applying it broadly or permanently can waste memory and actually hurt performance.

<a id="what-is-the-difference-between-animating-with-css-vs-with-javascript"></a>
### Q: What is the difference between animating with CSS vs. with JavaScript?
**Answer:** CSS animations/transitions are typically more performant for simple property changes since the browser can run many of them off the main thread, and need less code for common effects. JavaScript animation (`requestAnimationFrame`, or libraries like GSAP/Framer Motion) offers far more control — dynamic values, complex sequencing, and the ability to pause/reverse/inspect state mid-animation.

<a id="what-does-the-transition-delay-property-do-and-where-is-it-commonly-used"></a>
### Q: What does the `transition-delay` property do, and where is it commonly used?
**Answer:** It delays the start of a transition by a set amount of time after the triggering change happens — commonly used to stagger multiple elements' transitions one after another for a cascading visual effect.

---

<a id="css-variables-functions-preprocessors"></a>
## CSS Variables, Functions & Preprocessors

<a id="what-are-css-custom-properties-css-variables-and-how-do-you-declare-and-use-one"></a>
### Q: What are CSS custom properties (CSS variables), and how do you declare and use one?
**Answer:** Custom properties store a reusable value, declared with a `--` prefix and read with the `var()` function. Unlike preprocessor variables, they're live in the DOM — readable/changeable via JavaScript and responsive to the cascade.

**Example:**
```css
:root {
  --primary-color: #3b82f6;
}
.button {
  background-color: var(--primary-color);
}
```

<a id="what-is-the-difference-between-css-custom-properties-and-sassless-variables"></a>
### Q: What is the difference between CSS custom properties and Sass/Less variables?
**Answer:** Sass/Less variables are resolved at compile time — they become static, hardcoded values in the final CSS output. CSS custom properties are resolved at runtime by the browser, respect the cascade (can vary by where in the DOM they're read), and can be updated dynamically without recompiling anything.

<a id="what-does-the-calc-function-do-and-why-is-it-useful"></a>
### Q: What does the `calc()` function do, and why is it useful?
**Answer:** `calc()` lets you perform math directly in a CSS value, mixing different units — e.g. `width: calc(100% - 40px);` sizes an element to fill its container minus a fixed amount, something plain percentages or fixed units alone can't express.

<a id="what-does-the-clamp-function-do"></a>
### Q: What does the `clamp()` function do?
**Answer:** `clamp(min, preferred, max)` returns a value that's normally the "preferred" value, but never goes below "min" or above "max" — commonly used for fluid typography or spacing that scales with the viewport but stays within sensible bounds.

<a id="what-is-a-css-preprocessor-and-what-problem-does-it-solve"></a>
### Q: What is a CSS preprocessor, and what problem does it solve?
**Answer:** Preprocessors like Sass/SCSS and Less add features CSS historically lacked — nesting, variables, mixins, functions, and imports/partials — which compile down to plain CSS. They help organize larger stylesheets and reduce repetition, though native CSS has since adopted many similar features itself.

<a id="what-is-a-mixin-in-sass-and-how-does-it-differ-from-a-function"></a>
### Q: What is a mixin in Sass, and how does it differ from a function?
**Answer:** A mixin (`@mixin`, included with `@include`) is a reusable block of CSS declarations you can insert wherever needed, optionally parameterized. A function (`@function`) computes and returns a single value used inline within a property — mixins output whole rule blocks, functions output values.

<a id="what-is-the-difference-between-sasss-import-and-native-css-import"></a>
### Q: What is the difference between Sass's `@import` and native CSS `@import`?
**Answer:** Sass's `@import` (now deprecated in favor of `@use`/`@forward`) merges partial files together at compile time, with no extra runtime cost. Native CSS `@import` triggers an actual additional HTTP request at runtime (unless inlined by a build tool), which can hurt page load performance if overused.

<a id="how-does-native-css-nesting-compare-to-sass-nesting"></a>
### Q: How does native CSS nesting compare to Sass nesting?
**Answer:** Modern native CSS now supports nesting selectors directly (using `&` similarly to Sass) without a preprocessor, letting you write child/pseudo-class rules inside a parent selector's block. It closely mirrors what Sass has offered for years, though native nesting has its own specific syntax rules.

<a id="what-is-the-env-function-used-for-in-css"></a>
### Q: What is the `env()` function used for in CSS?
**Answer:** `env()` accesses environment variables defined by the user agent, most commonly used for device "safe area insets" on phones with notches — e.g. `padding-bottom: env(safe-area-inset-bottom);` keeps content clear of a phone's home-indicator bar.

<a id="how-would-you-implement-dark-mode-using-css-custom-properties"></a>
### Q: How would you implement dark mode using CSS custom properties?
**Answer:** Define semantic custom properties (`--bg-color`, `--text-color`) at `:root`, then override those same variable names inside a different scope — e.g. `[data-theme="dark"] { --bg-color: #111; --text-color: #eee; }` — toggled by adding/removing that attribute/class on a parent element, often respecting the OS `prefers-color-scheme` as a starting default.

---

<a id="advanced-architecture"></a>
## Advanced / Architecture

<a id="what-is-bem-and-what-problem-does-it-solve"></a>
### Q: What is BEM, and what problem does it solve?
**Answer:** BEM (Block, Element, Modifier) is a naming convention — `.block__element--modifier` — that keeps class names descriptive, flat (avoiding deep nesting/high specificity), and free of naming collisions, making large codebases easier to maintain without relying on strict source order or deeply nested selectors.

<a id="what-are-css-cascade-layers-layer-and-what-problem-do-they-solve"></a>
### Q: What are CSS cascade layers (`@layer`), and what problem do they solve?
**Answer:** `@layer` lets you explicitly define named layers of styles (e.g. `reset`, `base`, `components`, `utilities`) with a controlled priority order, independent of specificity or source order within each layer. This solves the classic problem of specificity wars — a low-specificity utility class no longer has to fight a highly-specific component rule, since layer order settles which wins first.

<a id="what-is-the-difference-between-utility-first-css-and-traditional-component-based-css"></a>
### Q: What is the difference between utility-first CSS and traditional component-based CSS?
**Answer:** Utility-first applies small, single-purpose classes directly in markup (`class="flex items-center p-4"`), avoiding custom CSS for most styling and keeping specificity uniformly low. Traditional/component-based CSS (BEM, CSS Modules) writes semantic, reusable class names tied to a component's meaning, with the actual styling defined separately.

<a id="what-are-css-modules-and-what-problem-do-they-solve"></a>
### Q: What are CSS Modules, and what problem do they solve?
**Answer:** CSS Modules automatically scope class names to the specific component/file they're defined in (via a build step generating unique class names), preventing global class name collisions across a large codebase — without needing manual naming conventions like BEM to avoid clashes.

<a id="what-is-the-difference-between-css-in-js-and-traditional-stylesheets"></a>
### Q: What is the difference between CSS-in-JS and traditional stylesheets?
**Answer:** CSS-in-JS (styled-components, Emotion) writes styles directly within JavaScript component files, often scoped automatically per component and able to use JS variables/props directly. Traditional stylesheets are separate `.css` files, generally simpler with better caching characteristics, but rely on naming conventions or tooling for scoping.

<a id="why-should-specificity-generally-trend-upward-through-a-stylesheet-rather-than-spike-unpredictably"></a>
### Q: Why should specificity generally trend upward through a stylesheet rather than spike unpredictably?
**Answer:** Ideally specificity stays flat or gradually increases from base/reset styles at the top to specific overrides/utilities at the bottom. Unpredictable spikes force later rules to be fought with `!important` or ID selectors, which is what causes long-term maintenance pain.

<a id="what-is-critical-css-and-why-is-it-used"></a>
### Q: What is critical CSS, and why is it used?
**Answer:** Critical CSS is the minimal subset of styles needed to render the above-the-fold content, inlined directly in `<head>` so the browser can paint visible content immediately without waiting for the full stylesheet to download — the rest loads asynchronously afterward.

<a id="what-is-the-difference-between-atomic-css-and-traditional-semantic-css-from-an-architecture-standpoint"></a>
### Q: What is the difference between atomic CSS and traditional semantic CSS from an architecture standpoint?
**Answer:** Atomic/utility CSS favors many small, single-purpose, reusable classes — less custom CSS overall, but more verbose markup. Semantic CSS favors fewer, more meaningful class names tied to component purpose — cleaner markup, but more custom CSS to write and maintain, with higher risk of duplication across similar components.

<a id="what-is-a-specificity-war-and-how-do-teams-typically-prevent-it"></a>
### Q: What is a "specificity war," and how do teams typically prevent it?
**Answer:** It happens when developers keep escalating selectors — adding IDs, `!important`, deeply nested selectors — just to override each other's styles, since each override needs higher specificity than the last. Teams prevent it with disciplined naming conventions (BEM), flat/low-specificity selectors, cascade layers, or utility-first approaches that avoid the problem by design.

<a id="what-is-the-difference-between-logical-properties-like-margin-inline-start-and-physical-properties-like-margin-left"></a>
### Q: What is the difference between logical properties (like `margin-inline-start`) and physical properties (like `margin-left`)?
**Answer:** Physical properties always refer to a fixed physical direction, regardless of writing mode. Logical properties (`margin-inline-start`, `padding-block-end`) refer to direction relative to the document's writing mode/direction — "start" is left in LTR languages but right in RTL — making layouts automatically adapt correctly for internationalization.

<a id="how-would-you-structure-a-large-css-codebase-to-keep-it-maintainable-over-time"></a>
### Q: How would you structure a large CSS codebase to keep it maintainable over time?
**Answer:** Organize by component/feature rather than one giant file, establish a consistent naming convention (BEM or utility classes) from the start, centralize design tokens (colors, spacing, typography) as custom properties or variables, keep selectors flat and low-specificity, and use cascade layers or CSS Modules to prevent styles from unintentionally leaking or colliding across the codebase.

---

<a id="performance-best-practices"></a>
## Performance & Best Practices

<a id="what-makes-some-css-selectors-more-expensive-to-match-than-others"></a>
### Q: What makes some CSS selectors more expensive to match than others?
**Answer:** Browsers match selectors right to left, so highly generic rightmost selectors combined with long ancestor chains require more comparisons across the DOM. In practice, modern browser engines are very well optimized, so selector performance rarely matters for typical sites — reducing overall CSS file size and avoiding excessive specificity/duplication usually matters more.

<a id="why-can-animating-widthheighttopleft-hurt-performance-compared-to-transform"></a>
### Q: Why can animating `width`/`height`/`top`/`left` hurt performance compared to `transform`?
**Answer:** Changing layout-affecting properties forces the browser to recalculate layout (reflow) and often repaint, potentially on every animation frame — expensive, especially with complex DOM trees. `transform` and `opacity` can be handled by the compositor alone, skipping layout and paint in many cases, making them far smoother.

<a id="what-is-the-difference-between-render-blocking-and-non-blocking-css-delivery"></a>
### Q: What is the difference between render-blocking and non-blocking CSS delivery?
**Answer:** By default, an external stylesheet linked via `<link rel="stylesheet">` blocks rendering until it downloads and is parsed. Techniques to reduce this: inlining critical CSS directly in `<head>`, and loading non-critical stylesheets asynchronously so they don't hold up the initial paint.

<a id="how-does-minifying-and-removing-unused-css-improve-performance"></a>
### Q: How does minifying and removing unused CSS improve performance?
**Answer:** Minification strips whitespace/comments, reducing download size. Removing unused CSS (via tools like PurgeCSS, or a framework's built-in purging) eliminates rules that never match anything on the page — often a much bigger win than minification alone on large, long-lived codebases.

<a id="what-is-the-impact-of-using-too-many-web-fonts-or-font-weights-on-performance"></a>
### Q: What is the impact of using too many web fonts or font weights on performance?
**Answer:** Each additional font file is a separate network request adding to total page weight, delaying text rendering, especially without `font-display: swap`. Limiting the number of font weights/styles actually used, and self-hosting/subsetting fonts, reduces this cost.

<a id="what-is-the-purpose-of-the-contain-and-content-visibility-css-properties-for-performance"></a>
### Q: What is the purpose of the `contain` and `content-visibility` CSS properties for performance?
**Answer:** `contain` tells the browser that an element's internal layout/paint/style won't affect anything outside it, letting the browser skip recalculating unaffected areas when that element changes. `content-visibility: auto` goes further, letting the browser entirely skip rendering work for offscreen content until it's about to become visible — a significant win for very long pages.

<a id="why-is-it-generally-recommended-to-avoid-deeply-nested-selectors-even-with-preprocessors-that-make-nesting-easy"></a>
### Q: Why is it generally recommended to avoid deeply nested selectors, even with preprocessors that make nesting easy?
**Answer:** Deep nesting tends to inflate specificity unnecessarily (each nested level often compiles into an increasingly specific compound selector) and produces longer, more expensive selectors that are harder to override or reuse — flatter, more modular selectors are easier to maintain at scale.

<a id="what-tools-would-you-use-to-audit-a-pages-css-performance"></a>
### Q: What tools would you use to audit a page's CSS performance?
**Answer:** Browser DevTools' Lighthouse panel for an overall performance/best-practices audit, the Coverage tab to find unused CSS, the Performance tab to check for layout thrashing during animations, and tools like PurgeCSS or a bundle analyzer to catch dead or duplicated styles before shipping.

---

<a id="behavioral-scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="how-would-you-debug-a-layout-where-an-elements-height-isnt-behaving-as-expected"></a>
### Q: How would you debug a layout where an element's height isn't behaving as expected?
**Answer:** Check the parent chain for `height: auto` breaking a percentage-based height, inspect computed styles in DevTools to see the actual applied box model values, check for margin collapsing, and check whether floated children are collapsing the parent's height without a clearfix.

<a id="how-would-you-approach-fixing-specificity-conflicts-in-a-large-legacy-css-codebase"></a>
### Q: How would you approach fixing specificity conflicts in a large, legacy CSS codebase?
**Answer:** Rather than escalating with more `!important`/IDs, identify and consolidate genuinely conflicting rules, gradually introduce a naming convention (like BEM) or cascade layers to establish clear priority, and make surgical, well-tested fixes to the specific conflict without touching unrelated styles.

<a id="how-would-you-build-a-layout-that-works-consistently-across-very-old-and-modern-browsers"></a>
### Q: How would you build a layout that works consistently across very old and modern browsers?
**Answer:** Use feature queries (`@supports`) to provide a Grid/Flexbox-based layout for modern browsers with a simpler fallback (floats or block-level stacking) for browsers lacking support, test against the project's actual required browser support matrix, and avoid relying on bleeding-edge features without a fallback where broad compatibility is required.

<a id="a-component-looks-fine-in-isolation-but-breaks-when-placed-inside-another-pages-layout-how-would-you-investigate"></a>
### Q: A component looks fine in isolation but breaks when placed inside another page's layout — how would you investigate?
**Answer:** Check for CSS specificity or class-name collisions from surrounding page styles overriding the component's own styles (a strong argument for CSS Modules or scoped styles), inspect for inherited properties (like `font-size` or `color`) leaking in from an ancestor, and check whether the component assumes a certain parent context that doesn't hold everywhere it's now used.

<a id="how-would-you-optimize-a-page-with-a-slow-css-heavy-initial-paint"></a>
### Q: How would you optimize a page with a slow, CSS-heavy initial paint?
**Answer:** Extract and inline critical, above-the-fold CSS directly into the HTML `<head>`, defer/async-load non-critical stylesheets, remove unused CSS rules from the bundle, and minimize expensive selectors or excessive `@import` chains that add extra network round-trips.

<a id="how-would-you-implement-a-design-systems-spacingcolor-scale-consistently-across-a-codebase"></a>
### Q: How would you implement a design system's spacing/color scale consistently across a codebase?
**Answer:** Define the scale as CSS custom properties (or design tokens) at a single source of truth, and reference those tokens everywhere instead of hardcoding raw values — making global updates a one-line change instead of a project-wide find-and-replace.

<a id="how-would-you-make-sure-a-ui-works-well-for-users-with-reduced-motion-preferences"></a>
### Q: How would you make sure a UI works well for users with reduced-motion preferences?
**Answer:** Wrap non-essential animations/transitions in an `@media (prefers-reduced-motion: reduce)` query, providing a reduced or instant alternative for users who've indicated a system-level preference against motion, which can trigger discomfort for some users (e.g. vestibular disorders).

<a id="how-would-you-approach-reviewing-a-teammates-css-pull-request"></a>
### Q: How would you approach reviewing a teammate's CSS pull request?
**Answer:** Check for unnecessary specificity escalation (IDs, `!important`) that could've been avoided, confirm responsive behavior across breakpoints, look for duplicated rules that could be consolidated into a shared class/variable, check color-contrast/accessibility of new UI, and verify the change doesn't accidentally leak styles to unrelated components.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to architecture.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
