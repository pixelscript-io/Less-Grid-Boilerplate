# CSS Grid Boilerplate

A lightweight 12-column CSS grid system built with CSS Grid and LESS.

![Grid System](http://i.imgur.com/KexAaDg.png)

## Installation

Simply just clone this repo to get started!

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
    <div class="one-half">Content</div>
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

Aligning content is easy.  The following classes will align your content vertically and horizontally, as you wish:

1. .center-v (Vertically center)
2. .center-h (Horizontally center)
3. .end-v (Vertically align to bottom)
4. .end-h (Horizontally align to right)

Just make sure you also add the `.grid` class as well.

Example markup:

```html
<div class="container">
  <div class="row">
    <div class="full grid center-v center-h">This is a full-width column and this text is centered.</div>
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

1. Grid system built by Joe Berthelot
2. Colors used are from [Open Color by yeun](https://github.com/yeun/open-color)
