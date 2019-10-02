# SVELTE-SORTABLE

>A Svelte wrapper component for [SortableJS](https://sortablejs.github.io/Sortable/).

## Install
`npm i -S svelte-sortable` or `yarn add svelte-sortable`

## Usage
```sveltehtml
<script>
    import SvelteSortable from "svelte-sortable"

    let items = [
        "wibble",
        "wobble",
        "wubble",
    ]
</script>

<SvelteSortable {items} let:item={item}>
    <span>{item}</span>
</SvelteSortable>
```