# CSS

## Selector

### Combinator selector

A combinator is something that defines the relationship between two or more selectors.

A CSS selector can contain more than one selector. Between the selectors, we can include a combinator, to create a more specific selection.

There are four different combinators in CSS:

Descendant combinator (space)
Child combinator (>)
Next sibling combinator (+)
Subsequent-sibling combinator (~)

descendant selector: Selects any element B that is inside A, no matter how deeply nested. Example:

> .parent p {
>
> color: blue;
>
> }

child selector: Selects only direct/immediate children of A. Example:

> .parent > p
> {
>
> }

adjacent sibling selector: Selects an element B that comes immediately after A — both at the same level (siblings).. Example:

> h2 + p {
>
> }

general sibling selector: Selects all elements B that come after A, not just the first one, as long as they’re siblings. Example:

> h2 ~ p {
>
> }

### Compound selector
