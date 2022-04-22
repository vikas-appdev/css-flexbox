## Responsive CSS & Flexbox

- flex shorthand
- flex basis, grow and shrink
- align-items
- flex-wrap
- align-content and align-self
- justify-content
- flex-direction
- media queries (IMPORTANT)


### Introduction to CSS Flexbox

#### What is it?

Flexbox is a one-dimensional layout method for laying out items in rows or columns.

Flexbox is a recent addition to CSS included to address common layout frustratation.

#### Why 'flex' ?

flexbox allows us to disribute space dynamically across elements of an unknown size, hence the term 'flex'.


#### FLEX DIRECTION

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="css/app.css">
    <title>Document</title>
</head>

<body>

    <h1>Flexbox Example</h1>
    <section id="container">
        <div style="background-color: #80ffdb;"></div>
        <div style="background-color: #64dfdf;"></div>
        <div style="background-color: #48bfe3;"></div>
        <div style="background-color: #5390d9;"></div>
        <div style="background-color: #6930c3;"></div>

    </section>

</body>

</html>
```

app.css

```css
body {
    font-family: 'Open Sans', sans-serif;
}

h1 {
    text-align: center;
}

#container {
    background-color: #003049;
    width: 90%;
    height: 500px;
    margin: 0 auto;
    border: 5px solid #003049;
    display: flex;
    flex-direction: column-reverse;

}

#container div {
    width: 200px;
    height: 200px;
}
```