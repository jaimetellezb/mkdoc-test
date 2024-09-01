# Usage

This section covers the basic usage of the ListView Widget, including initialization, data binding, and event handling.

## Basic Setup

Here's a simple example to get you started:

```html
<div id="list-container"></div>

<script>
  const myData = ['Item 1', 'Item 2', 'Item 3'];

  const listView = new ListView({
      data: myData,
      container: '#list-container',
  });

  listView.render();
</script>
```