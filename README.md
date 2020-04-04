## Emmet abbreviations list

This repo is a list of the most useful emmet abbreviations for working in HTML or HTML Native files

## Table of contents

- [HTML Boilerplate](#html-boilerplate)
- [Mock text](#mock-text)
- [Tags](#tags)
  - [Tags with classes](#tags-with-classes)
  - [Tags with ids](#tags-with-ids)
  - [Tags with multiple classes and ids](#tags-with-multiple-classes-and-ids)
  - [Tags with hard-coded values](#tags-with-hard-coded-values)
- [Div shortcuts](#div-shortcuts)
- [Custom attributes](#custom-attributes)
  - [Div with a custom attribute](#div-with-a-custom-attribute)
  - [Div with a custom attribute and class](#div-with-a-custom-attribute-and-class)
- [Nesting child elements](#nesting-child-elements)
  - [Nesting multiple children](#nesting-multiple-children)
- [Creating multiple tags](#creating-multiple-tags)
  - [Creating multiple tags with hard-coded values](#creating-multiple-tags-with-hard-coded-values)
  - [Creating multiple tags with numbered values](#creating-multiple-tags-with-numbered-values)
- [Creating sibling elements](#creating-sibling-elements)
  - [Nesting child elements in sibling elements](#nesting-child-elements-in-sibling-elements)
- [Forms](#forms)
  - [Inputs](#inputs)
- [Other sources](#other-sources)

# HTML Boilerplate

`!` or `html:5` - generate an HTML Boilerplate

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

# Mock text

`lorem[number]` -generate mock text with specified length

```html
lorem5 -> Lorem ipsum dolor sit amet.
lorem -> Lorem, ipsum dolor sit amet consectetur adipisicing...
```

# Tags

`[tag_name]` - generate a tag by typing its name

```html
div -> <div></div>
span -> <span></span>
img -> <img src="" alt="">
a -> <a href=""></a>
link -> <link rel="stylesheet" href="">
```

## Tags with classes

`[tag_name].[class_name]` - generate a tag with a defined class name

```html
div.container -> <div class="container"></div>
span.wrapper -> <span class="wrapper"></span>
```

## Tags with ids

`[tag_name].[id_name]` - generate a tag with a defined id

```html
div#container -> <div id="container"></div>
span#wrapper -> <span id="wrapper"></span>
```

## Tags with multiple classes and ids

`[tag_name].[class_name]#[id_name]` - generate a tag with defined class name(s) and an id(s)

```html
div.class-1.class-2#id-1 -> <div class="class-1 class-2" id="id-1"></div>
```

## Tags with hard-coded values

`[tag_name]{value}` - generate a tag with a defined hard-coded value

```html
div{hello} -> <div>hello</div>
p.muted{hello again} -> <p class="muted">hello again</p>
```

# Div shortcuts

`.[class_name]` or `#[id_name]` - generate a div with a defined class name or an id

```html
.class -> <div class="class"></div>
#id -> <div id="id"></div>
```

# Custom attributes

`[tag_name][attribute_name]` - generate a tag with a custom attribute

```html
button[type] -> <button type=""></button>
button[type="button"] -> <button type="button"></button>
```

## Div with a custom attribute

`[attribute_name]` - generate a div with a custom attribute

```html
[data-selected] -> <div data-selected=""></div>
```

## Div with a custom attribute and class

`[attribute_name].[class_name]` - generate a div with a custom attribute and a defined class name

```html
[data-selected].active -> <div data-selected="" class="active"></div>
```

# Nesting child elements

`[parent]>[child]` - generate a tag with a defined element nested as its child

```html
.purple>span.magneta -> <div class="purple"><span class="magneta"></span></div>
```

## Nesting multiple children

`[parent]>[child]>[child]>...` - generate a tag with a multiple defined elements nested as its children and grandchildren

```html
header>nav>ul ->

<header>
  <nav>
    <ul></ul>
  </nav>
</header>
```

# Creating multiple tags

`[tag_name]*[number]` - generate a defined number of tags

```html
li*3 ->

<li></li>
<li></li>
<li></li>
```

## Creating multiple tags with hard-coded values

`[tag_name]*[number]{value}` - generate a defined number of tags with a specified hard-coded value

```html
li*3{emmet is easy} ->

<li>emmet is easy</li>
<li>emmet is easy</li>
<li>emmet is easy</li>
```

## Creating multiple tags with numbered values

`[tag_name]*[number]{$}` - generate a defined number of tags with a dynamically changing number value

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

# Creating sibling elements

`[tag_name]+[tag_name]+[tag_name]+...` - generate tags which compose sibling relationship in the document

```html
header+main+footer ->

<header></header>
<main></main>
<footer></footer>
```

## Nesting child elements in sibling elements

- `[tag_name]>[tag_name]^[tag_name]+[tag_name]` - generate a tag with one child element and two siblings

- `([tag_name]>[tag_name])+[tag_name]+[tag_name]` - alternative grouping syntax

```html
header>nav^main+footer ->

<header>
  <nav></nav>
</header>
<main></main>
<footer></footer>
```

# Forms

`form:[form_method]` - generate a form with a defined method

```html
form:post -> <form action="" method="post"></form>
```

## Inputs

`input:[input_type]` - generate an input with a defined type

```html
form:post>.group>input:text ->

<form action="" method="post">
  <div class="group">
    <input type="text" name="" id="">
  </div>
</form>
```

# Other sources

- [Emmet cheatsheet](https://docs.emmet.io/cheat-sheet)
- [Emmet docs](https://docs.emmet.io/)
- [Emmet repo](https://github.com/emmetio/emmet)
