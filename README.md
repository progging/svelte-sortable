# SVELTE-SORTABLE

>A Svelte wrapper component for [SortableJS](https://sortablejs.github.io/Sortable/).

## Install
`npm i -S svelte-sortable` or `yarn add svelte-sortable`

## Usage
```sveltehtml
<script>
    import { Sortable, MultiDrag } from "svelte-sortable"

    // In case multiselection is to be used 
    Sortable.mount(new MultiDrag());

    let items = [
        "foo",
        "bar",
        "baz",
    ]

    function onChange() {
        //`items` are mutated
        console.log(items)
    }

</script>

<Sortable {items}
          let:item={item}
          on:change={onChange}>
    <div>
        {item}
    </div>
</Sortable>
```
