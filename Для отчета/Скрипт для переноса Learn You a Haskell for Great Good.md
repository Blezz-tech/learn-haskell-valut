```js
document.querySelector('#content').style.width = 'auto';

[...document.querySelectorAll('[name="code"]')].forEach(item => {
    item.style.display = "block";
    const text = item.innerText;
    item.innerHTML = `<code>${item.innerHTML}</code>`;
});

[...document.querySelectorAll('#content>p>span')].forEach(item => {
    item.outerHTML = `<code>${item.innerHTML}</code>`;
});

[...document.querySelectorAll('.dp-highlighter')].forEach(item => {
    item.style.display = "none";
});

[...document.querySelectorAll('#content>p>em')].forEach(item => {
    item.outerHTML = item.outerHTML.replace(/em/g,"strong");
});
```