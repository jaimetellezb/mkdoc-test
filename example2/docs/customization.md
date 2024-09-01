# Customization

The ListView Widget can be extensively customized to match your application's needs.

## Styling

You can customize the appearance using CSS:

```css
.item {
    padding: 10px;
    border-bottom: 1px solid #ccc;
}

.item h3 {
    font-size: 18px;
    color: #333;
}

.item p {
    font-size: 14px;
    color: #666;
}
```

### Configuration Options

Configure the widget's behavior using the following options:

```js
const listView = new ListView({
    data: myData,
    container: '#list-container',
    orientation: 'horizontal', // 'vertical' or 'horizontal'
    itemHeight: 60,
    itemWidth: 200,
    bufferSize: 10, // Number of items to keep in the buffer for virtual scrolling
    onItemRender: (item, index) => {
        console.log(`Rendering item at index ${index}`);
    },
});

listView.render();

class CustomListView extends ListView {
    constructor(options) {
        super(options);
    }

    render() {
        console.log('Custom render logic');
        super.render();
    }
}

const customListView = new CustomListView({
    data: myData,
    container: '#list-container',
});

customListView.render();
```
