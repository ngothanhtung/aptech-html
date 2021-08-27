# CSS Grid Layout Module

[Tham khảo: https://www.w3schools.com/css/css_grid.asp](https://www.w3schools.com/css/css_grid.asp)

The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

> Example

```css
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  background-color: #2196f3;
  padding: 10px;
}
.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}
```

```html
<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>
  <div class="grid-item">7</div>
  <div class="grid-item">8</div>
  <div class="grid-item">9</div>
</div>
```

## Display Property

An HTML element becomes a grid container when its **display** property is set to **grid** or **inline-grid**.

> Example

```css
.grid-container {
  display: grid;
}
```

```css
.grid-container {
  display: inline-grid;
}
```

## Grid Columns

The vertical lines of grid items are called columns.

<div style="background-color: whitesmoke; padding: 24px; margin-bottom: 24px">

![alt text](https://www.w3schools.com/css/grid_columns.png)

</div>

## Grid Rows

The horizontal lines of grid items are called rows.

<div style="background-color: whitesmoke; padding: 24px; margin-bottom: 24px">

![alt text](https://www.w3schools.com/css/grid_rows.png)

</div>

## Grid Gaps

The spaces between each column/row are called gaps.

<div style="background-color: whitesmoke; padding: 24px; margin-bottom: 24px">

![alt text](https://www.w3schools.com/css/grid_gaps.png)

</div>
You can adjust the gap size by using one of the following properties:

- grid-column-gap
- grid-row-gap
- grid-gap

> Example

```css
.grid-container {
  display: grid;
  grid-column-gap: 50px;
  grid-gap: 50px 100px;
}
```

## Grid Lines

- The lines between columns are called column lines.
- The lines between rows are called row lines.

<div style="background-color: whitesmoke; padding: 24px; margin-bottom: 24px">

![](https://www.w3schools.com/css/grid_lines.png)

</div>

Refer to line numbers when placing a grid item in a grid container:

> Example

Place a grid item at column line 1, and let it end on column line 3:

```css
.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
```

> Example

Place a grid item at row line 1, and let it end on row line 3:

```css
.item1 {
  grid-row-start: 1;
  grid-row-end: 3;
}
```
