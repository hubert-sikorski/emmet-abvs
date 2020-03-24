## Emmet abbreviations list

This repo is a list of the most useful emmet abbreviations for working in HTML or HTML Native files

## Table of contents

- [HTML Boilerplate](#html-boilerplate)
- [Tags](#tags)
  - [Tags with classes](#tags-with-classes)
  - [Tags with ids](#tags-with-ids)
  - [Tags with multiple classes and ids](#tags-with-multiple-classes-and-ids)
- [Div shortcuts](#div-shortcuts)
- [Custom attributes](#custom-attributes)
  - [Div with custom attribute](#div-with-custom-attribute)

# HTML Boilerplate

- `!` - generate HTML Boilerplate

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>

</body>
</html>
```

# Tags

- `[tag_name]` - generate a tag by typing its name

```html
div -> <div></div>
span -> <span></span>
img -> <img src="" alt="">
a -> <a href=""></a>
link -> <link rel="stylesheet" href="">
```

## Tags with classes

- `[tag_name].[class_name]`

```html
div.container -> <div class="container"></div>
span.wrapper -> <span class="wrapper"></span>
```

## Tags with ids

- `[tag_name].[id_name]`

```html
div#container -> <div id="container"></div>
span#wrapper -> <span id="wrapper"></span>
```

## Tags with multiple classes and ids

- `[tag_name].[class_name]#[id_name]`

```html
div.class-1.class-2#id-1 -> <div class="class-1 class-2" id="id-1"></div>
```

# Div shortcuts

- `.[class_name]` or `#[id_name]`

```html
.class -> <div class="class"></div>
#id -> <div id="id"></div>
```

# Custom attributes

- `[tag_name][attribute_name]`

```html
button[type] -> <button type=""></button>
button[type="button"] -> <button type="button"></button>
```

## Div with custom attribute

- `[attribute_name]`

```html
[data-selected] -> <div data-selected=""></div>
```
