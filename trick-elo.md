### tự động chọn 100 cho tất cả các ô <select> có class ratinginput
```js
allow pasting

document.querySelectorAll('select.ratinginput').forEach(select => {
    select.value = "100";
    select.dispatchEvent(new Event('change', { bubbles: true }));
});
```
