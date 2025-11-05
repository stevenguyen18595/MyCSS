# CSS

## Selector

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

adjacent sibling selector: Selects an element B that comes immediately after A — both at the same level (siblings).. ex: h2 + p {}

general sibling selector: Selects all elements B that come after A, not just the first one, as long as they’re siblings. ex: h2 ~ p {}
