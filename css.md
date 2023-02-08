 # CSS Questions <!-- omit from toc -->

## Table of Contents
- [Table of Contents](#table-of-contents)
- [Q. Explain the box model in CSS?](#q-explain-the-box-model-in-css)
- [Q. What are CSS variables?](#q-what-are-css-variables)
- [Q. What are the different `position` values an element can take?](#q-what-are-the-different-position-values-an-element-can-take)

<br>

## Q. Explain the box model in CSS?

The box model in CSS refers to the concept that every HTML element is treated as a rectangular box that has content, padding, borders, and margins.

* Content: The content of the box is the actual content of the HTML element, such as text or images.

* Padding: The padding of the box is the space between the content and the border. The padding is transparent and is used to create space around the content.

* Border: The border of the box surrounds the content and padding. The border can have different styles, such as color, width, and style (e.g. solid, dotted, etc.).

* Margin: The margin of the box is the space outside the border. The margin is used to create space between elements.

The size and position of the box are determined by the content, padding, borders, and margins, and can be controlled using CSS properties such as `width`, `height`, `padding`, `border`, and `margin`.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are CSS variables?
CSS variables, also known as CSS custom properties, are values that can be assigned to specific CSS properties. CSS variables are similar to variables in programming languages and allow you to store values that can be reused throughout a stylesheet.

CSS variables are declared using the `--` syntax followed by a name, and they can be used in a CSS declaration by using the `var()` function. For example:

```css
:root {
  --primary-color: #ff0000;
}

.header {
  background-color: var(--primary-color);
}
```

In this example, a CSS variable named `--primary-color` is declared with the value `#ff0000`. This variable can then be used as the value for the `background-color` property of the `.header` class.

CSS variables offer several benefits, such as:

* Reusability: By using variables, you can define values in one place and reuse them throughout a stylesheet.

* Maintainability: By using variables, you can make global changes to your stylesheet by changing a single value.

* Improved organization: By grouping related values together in variables, you can make your stylesheet easier to read and maintain.

Overall, CSS variables are a useful tool for making your stylesheets more efficient and manageable.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the different `position` values an element can take?

What are the different `position` values an element can take?

* **Static**

`position: static` is the default value. An element with `position: static` is not positioned in any special way.

* **Relative**

`position: relative` behaves the same as static unless you add some extra properties. Setting the `top`, `right`, `bottom` and `left` properties of a relatively-positioned element will cause it to be adjusted away from its normal position. This means that the new position (determined by `top`, `right`, `bottom`, `left`) is relative to the original (static) position.

```css
#something {
  position: relative; /* i'm gonna move this element from its original spot */
  top: -10px; /* push this 10px up to the top */
  left: 20px; /* push this 20px to the right */
}
```

* **Fixed**

A fixed element is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled (think of a modal window). As with relative, the `top`, `right`, `bottom`, and `left` properties are used.

* **Absolute**

`position: absolute` behaves like `fixed` except relative to the nearest positioned ancestor instead of relative to the viewport. If an absolutely-positioned element has no positioned ancestors, it uses the document body, and still moves along with page scrolling. Remember, a "positioned" element is one whose position is anything except `static`.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>