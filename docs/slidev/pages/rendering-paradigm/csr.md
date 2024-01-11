---
---

# Client-side rendering

![](/assets/csr.png){width=70%}

```html {all|9,11}
<!-- index.html -->
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <div id="body"></div>
  </body>
  <script src="index.js"></script>
</html>
```

```js
// index.js
React.render(<App />, document.getElementById('body'))s
```