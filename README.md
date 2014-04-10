## About listfilter.js

Listfilter creates a fast, case-insensitive text filter against a list of HTML elements on a page. Sometimes you just need a little thing to do a thing, you know?

## Requirements

* jQuery

## Sample use

This finds an unordered list of class `my-list`, and prepends it with a text input that filters the `li` elements in the list.

```var filter = ListFilter({
    listContainer: 'ul.my-list',
    filterItemClass: 'li'
});

```

This creates a text input inside an existing page element with ID `filter-list-input-container`. The text input filters children of class `filter-item` inside a parent of ID `filterable-list`. The child elements may be grouped inside blocks of class `filter-block`, and if no children inside a block match the text filter, the entire block is hidden as well.

```var filter = ListFilter({
    inputContainer: '#filter-list-input-container',
    listContainer: '#filterable-list',
    filterItemClass: '.filter-item',
    filterBlockClass: '.filter-block'
});
```
