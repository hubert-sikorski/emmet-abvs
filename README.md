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
  - [Div with custom attribute and class](#div-with-custom-attribute-and-class)
- [Nesting child elements](#nesting-child-elements)
  - [Nesting multiple children](#nesting-multiple-children)
- [Creating multiple tags](#creating-multiple-tags)
  - [Creating multiple tags with hard-coded values](#creating-multiple-tags-with-hard-coded-values)
  - [Creating multiple tags with numbered values](#creating-multiple-tags-with-numbered-values)

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

## Div with custom attribute and class

- `[attribute_name].[class_name]`

```html
[data-selected].active -> <div data-selected="" class="active"></div>
```

# Nesting child elements

- `[parent]>[child]`

```html
.purple>span.magneta -> <div class="purple"><span class="magneta"></span></div>
```

## Nesting multiple children

- `[parent]>[child]>[child]>...`

```html
header>nav>ul ->
<header>
  <nav>
    <ul></ul>
  </nav>
</header>
```

# Creating multiple tags

- `[tag_name]*[number]`

```html
li*3 ->
<li></li>
<li></li>
<li></li>
```

## Creating multiple tags with hard-coded values

- `[tag_name]*[number]{value}`

```html
li*3{emmet is easy} ->
<li>emmet is easy</li>
<li>emmet is easy</li>
<li>emmet is easy</li>
```

## Creating multiple tags with numbered values

- `[tag_name]*[number]{$}`

```html
li*3{item $} ->
<li>item 1</li>
<li>item 2</li>
<li>item 3</li>

li*3.class-${item $} ->
<li class="class-1">item 1</li>
<li class="class-2">item 2</li>
<li class="class-3">item 3</li>
```
