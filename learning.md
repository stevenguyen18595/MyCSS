# CSS

## Selector

### Combinator selector

A combinator defines the **relationship between two or more selectors**. CSS selectors can contain multiple selectors with combinators between them to create more specific selections.

#### Definition

Combinators are special characters or spaces that indicate how elements relate to each other in the HTML structure, allowing you to target elements based on their position relative to other elements.

There are four different combinators in CSS:

#### Types of Combinators:

##### 1. Descendant Combinator (space)

- **Syntax**: `A B`
- **Purpose**: Selects any element B that is inside A, no matter how deeply nested
- **Example**:

```css
.parent p {
  color: blue;
}
/* Selects all <p> elements inside any element with class 'parent' */
```

##### 2. Child Combinator (>)

- **Syntax**: `A > B`
- **Purpose**: Selects only direct/immediate children of A
- **Example**:

```css
.parent > p {
  font-weight: bold;
}
/* Selects only <p> elements that are direct children of elements with class 'parent' */
```

##### 3. Adjacent Sibling Combinator (+)

- **Syntax**: `A + B`
- **Purpose**: Selects element B that comes immediately after A (both at the same level as siblings)
- **Example**:

```css
h2 + p {
  margin-top: 0;
}
/* Selects the first <p> element that immediately follows an <h2> */
```

##### 4. General Sibling Combinator (~)

- **Syntax**: `A ~ B`
- **Purpose**: Selects all elements B that come after A, as long as they're siblings
- **Example**:

```css
h2 ~ p {
  color: gray;
}
/* Selects all <p> elements that come after an <h2> at the same level */
```

### Compound selector

A CSS compound selector is a sequence of simple selectors written together **without any combinators** (like spaces, +, ~, or >) in between. It targets a single element that must meet multiple conditions simultaneously.

#### Definition

A compound selector combines multiple simple selectors to create more specific targeting rules for a single element.

#### Key Characteristics:

- **Combines Multiple Conditions**: Target an element based on multiple criteria at once (type, class, ID, and/or attributes)
- **No Combinators**: No spaces or special characters between selectors (which would indicate relationships between different elements)
- **Higher Specificity**: More specific than individual simple selectors, taking precedence in case of conflicts

#### Examples:

```css
/* Targets div elements with class 'container' and id 'main' */
div.container#main {
  background-color: blue;
}

/* Targets paragraph elements with both 'highlight' and 'important' classes */
p.highlight.important {
  color: red;
  font-weight: bold;
}

/* Targets input elements with type 'text' and class 'form-control' */
input[type="text"].form-control {
  border: 1px solid #ccc;
}
```
