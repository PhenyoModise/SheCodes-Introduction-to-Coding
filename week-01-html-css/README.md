# Week 1: HTML and CSS

## HTML fundamentals

HTML provides the structure and content of a web page.

| Element | Purpose |
| --- | --- |
| `<h1>` | Main heading |
| `<strong>` | Important text, typically bold |
| `<em>` | Emphasized text, typically italic |
| `<p>` | Paragraph |
| `<br>` | Line break |
| `<hr>` | Thematic break |
| `<ul>` | Unordered list |
| `<ol>` | Ordered list |
| `<li>` | List item |
| `<a href="...">` | Hyperlink |
| `<img src="..." alt="...">` | Image |

### Links and images

Attributes provide extra information about an HTML element. `href` identifies a link destination; `src` identifies an image resource.

```html
<a href="https://www.shecodes.io/">SheCodes</a>
<img src="coffee.jpg" alt="A cup of coffee" />
```

## CSS fundamentals

CSS controls presentation. Rules use selectors, properties and values.

```css
h1 {
  color: blueviolet;
}

p {
  color: green;
}
```

### Classes and selectors

A class can target a subset of elements rather than every element of the same type.

```html
<li class="premium">SheCodes</li>
<li class="free">SheCodes workshop</li>
```

```css
.premium {
  color: purple;
}
```

### Properties and layout

- `color` and `background` control text and background colours.
- `text-transform` changes text casing; `font-style` controls italics.
- `display: block` and `margin: 0 auto` can centre a fixed-width image.
- `padding` adds space inside an element; `margin` adds space outside it.
- One to four padding or margin values set sides in CSS shorthand order.
- `:hover` changes styling while a pointer is over an element.
- `cursor: pointer` indicates a clickable element.
- `transition` smooths changes between styles.
- Browsers supply default CSS, which custom styles can override.

```css
button {
  display: block;
  margin: 20px auto;
  padding: 15px 20px;
  background: transparent;
  transition: all 200ms ease-in-out;
}
button:hover {
  background: white;
  color: pink;
  cursor: pointer;
}
```

### Container elements

`<div>` is a block-level container and `<span>` is an inline container. Both can be styled using classes.

## Related project

[SheCodes landing page](../projects/shecodes-landing-page/)
