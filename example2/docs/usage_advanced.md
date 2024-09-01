# Advanced Usage

Explore advanced scenarios including custom layouts, asynchronous data loading, and performance tuning.

## Custom Item Layouts

Define a custom layout template for list items:

```javascript
const listView = new ListView({
    data: myData,
    container: '#list-container',
    itemTemplate: (item) => `
        <div class="item">
            <h3>${item.name}</h3>
            <p>Details: ${item.details}</p>
        </div>
    `,
});
```

### Asynchronous Data Loading

Load data asynchronously into the ListView:

```js

listView.render();


fetch('/api/data')
  .then(response => response.json())
  .then(data => {
      listView.updateData(data);
  });


  const listView = new ListView({
    data: myLargeData,
    container: '#list-container',
    virtualScroll: true, // Enables virtual scrolling for large lists
    itemHeight: 50,      // Specify fixed item height for better performance
});

listView.render();
```

