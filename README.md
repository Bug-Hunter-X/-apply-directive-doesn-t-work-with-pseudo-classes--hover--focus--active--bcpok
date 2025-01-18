# Tailwind CSS @apply Directive Bug with Pseudo-classes

This repository demonstrates a bug where the `@apply` directive in Tailwind CSS fails to apply styles with pseudo-classes such as `hover`, `focus`, or `active`.

## Bug Description

The `@apply` directive, when used with a class containing a pseudo-class selector (e.g., `hover:bg-blue-500`), does not correctly apply the styles to the target element. This results in the styles not being applied on hover, focus, or active states.

## Reproduction Steps

1. Clone the repository.
2. Open `bug.html` in your browser.
3. Observe that the button's background color does not change on hover, despite the use of `@apply hover:bg-blue-500`.

## Solution

The solution is to avoid using `@apply` with pseudo-class selectors. Instead, directly apply the class to the element, or use the appropriate directives. Refer to `solution.html` for the corrected code.