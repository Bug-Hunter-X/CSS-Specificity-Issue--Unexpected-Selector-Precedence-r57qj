# CSS Specificity Issue: Unexpected Selector Precedence

This repository demonstrates a subtle bug related to CSS selector specificity. The bug arises from an unexpected interaction between class and ID selectors when combined with a descendant combinator.

## Bug Description

The bug lies in the understanding and application of CSS specificity rules when combining class and ID selectors. A common expectation is that the ID selector will always have higher specificity. However, in some cases involving combined selectors, the combined selector will have higher specificity. 

## How to Reproduce

1.  Clone this repository.
2. Open `bug.css` to see the problematic code. Note that the rule `.container #container` surprisingly overrides both `.container` and `#container`.
3. Open `bugSolution.css` to see the solution that addresses the problem.