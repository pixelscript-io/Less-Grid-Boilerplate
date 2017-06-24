# CSS Grid Boilerplate

A lightweight 12-column CSS grid system built with CSS Grid and LESS.

![Grid System](http://i.imgur.com/xCBYnOp.png)

## Installation

Simply just clone this repo to get started! View `example.html` for a variety of different possibilities.

## Usage

The only requirements are that the columns are nested in a `.container` and a `.row`.  The markup is simple and straightforward:

```html
<div class="container">
  <div class="row">
    <div class="full">This is a full-width column.</div>
  </div>
</div>
```

To create a two-column layout with a header and footer:

```html
<div class="container">
  <div class="row">
    <div class="full">Header</div>
  </div>
  <div class="row">
    <div class="two-thirds">Content</div>
    <div class="one-third">Sidebar</div>
  </div>
  <div class="row">
    <div class="full">Footer</div>
  </div>
</div>
```

The layout comes with a max-width of 960px, column and row-gap of 20px out of the box.  To change or remove these variables, just modify them in `css/sizes.less`.

## The Classes

The following classes are used to set the width of your columns:

1. .full (12/12 Columns)
2. .one-half (6/12 Columns)
3. .two-thirds (8/12 Columns)
4. .one-third (4/12 Columns)
5. .one-fourth (3/12 Columns)
6. .one-sixth (2/12 Columns)

Creating a `<div>` without one of the above classes will automatically span it 1/12 columns.

## Helper Classes

#### Content Alignment

Aligning content is easy.  The following classes will align your content vertically and horizontally, as you wish:

1. .content-center-v (Vertically center content)
2. .content-center-h (Horizontally center content)
3. .content-end-v (Vertically align content to bottom)
4. .content-end-h (Horizontally align content to right)

Just make sure you also add the `.grid` class as well.

Example markup:

```html
<div class="container">
  <div class="row">
    <div class="full grid center-v center-h">This is a full-width column and this text is centered.</div>
  </div>
</div>
```

#### Column Alignment

1. .middle (Align a column to the middle of the grid)

Use the `.middle` class to align the column to the middle of the layout.  This only works on classes: `.one-half .two-thirds .one-third .one-sixth`.

#### Fixed Header & Footer

1. .top (Align a row to the top of the layout)
2. .bottom (Align a row to the bottom of the layout)

If you want to position an element to the top or bottom of your layout, add the `.grid` class to your `.container` and add either `.top` or `.bottom` to your `.row`.  Example markup:

```html
<div class="container grid">
  <div class="row top">
    <div class="full">Header</div>
  </div>
  <div class="row">
    <div class="two-thirds">Content</div>
    <div class="one-third">Sidebar</div>
  </div>
  <div class="row bottom">
    <div class="full">Footer</div>
  </div>
</div>
```

## Contributing

1. Fork it!
2. Create your new branch: `git checkout -b my-new-branch`
3. Commit your changes: `git commit -am 'Add some stuff'`
4. Push to the branch: `git push origin my-new-branch`
5. Submit a pull request :D

## Credits

Grid system built by Joe Berthelot.
