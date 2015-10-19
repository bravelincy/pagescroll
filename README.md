# pagescroll
移动端全屏插件

## 使用方法
```javascript
pageScroll({
    container: '.pages',
    direction: 'vertical',
    effect: 'ease',
    start: function (index) {
        console.log('start', this, index);
    },
    end: function (index, prevIndex, prevPage) {
        console.log('end', this, index, prevIndex, prevPage);
        this.classList.add('active');
        prevPage.classList.remove('active');
    }
});
```
