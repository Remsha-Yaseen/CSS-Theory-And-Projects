# CSS Attribute Selectors Cheat Sheet

A quick-reference guide for targeting HTML elements based on attributes (`href`, `title`, `lang`, `type`) and specific value patterns.

---

## 1. Link & General Attribute Selectors

### Presence Selector (`[attr]`)
Targets elements that contain the specified attribute, regardless of its value.

```html
<a href="[https://www.freecodecamp.org](https://www.freecodecamp.org)">Link with href</a>
<a>No href</a>

a[href] {
  color: blue;
  text-decoration: underline;
}
```


### Specific Attribute Match
Targets elements containing a specific attribute like `title.`

```html
<a href="#" title="Tooltip">Link with title</a>
<a href="#">Normal link</a>

a[title] {
  font-weight: bold;
  text-decoration: none;
}
```


#### Combined Selectors
Chains multiple attribute selectors to target elements that meet all conditions.

```html
<a href="#" title="Info">Href + Title</a>
<a href="#">Only href</a>

a[href][title] {
  color: green;
}
```


## 2. Advanced Pattern Matching
**Exact Word Match (~=)**
Targets an attribute value containing a specific whole word within a space-separated list.

```html
<a class="link primary">Primary link</a>
<a class="link secondary">Secondary link</a>

a[class~="primary"] {
  color: red;
  font-weight: bold;
}
```


**Prefix Match (^=)**
Targets elements whose attribute value starts with the specified string.

```html
<a href="[https://www.freecodecamp.org](https://www.freecodecamp.org)">HTTPS link</a>
<a href="[http://www.freecodecamp.org](http://www.freecodecamp.org)">HTTP link</a>


a[href^="https://"] {
  color: green;
  text-decoration: underline;
}
```


**Suffix Match ($=)**
Targets elements whose attribute value ends with the specified string.

```html
<a href="photo.jpg">Image link</a>
<a href="index.html">HTML link</a>

a[href$=".jpg"] {
  color: darkgreen;
  text-decoration: underline dotted;
}
```

**Substring Match (*=)**
Targets elements whose attribute value contains the specified string anywhere inside it.

```html
<a href="[https://www.freecodecamp.org](https://www.freecodecamp.org)">Secure link</a>
<a href="page.html">Local link</a>

a[href*="https"] {
  color: teal;
}
```


## 3. Language & Custom Data Attributes
**Language Selector (lang)**
Styles elements based on the native HTML language configuration.

```html
<p lang="en">English text</p>
<p lang="fr">French text</p>

p[lang="en"] {
  font-style: italic;
}
```


## Language & Custom Data Selector (data-*)
**Styles elements based on custom data attributes used to store extra configuration.**

```html
<div data-lang="fr">French content</div>
<div data-lang="en">English content</div>

div[data-lang="fr"] {
  color: blue;
}
```

## 4. Ordered Lists & List Types
**List Type Selector (type)**
Targets ordered lists (<ol>) based on their numbering style attribute.

```html
<ol type="A">
  <li>Alpha</li>
  <li>Beta</li>
</ol>

<ol type="i">
  <li>One</li>
  <li>Two</li>
</ol>

/* Target uppercase alphabetical numbering */
ol[type="A"] {
  color: purple;
  font-weight: bold;
}

/* Target lowercase Roman numerals */
ol[type="i"] {
  color: green;
}
```
