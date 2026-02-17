# 🔗 Lists and Links: Navigation & Structure
In this section, we transition from simple text boxes to interactive elements. Lists provide the structure for data and navigation, while links provide the connectivity of the web.

----

### 1. Styling Lists
By default, browsers add specific markers (bullets or numbers) and padding to lists. We can control these using `list-style.`

* `list-style-type:` Changes the marker (e.g., `square`, `circle, decimal`, or `none`).

* `list-style-position:` Determines if the marker sits `inside` or `outside` the list item box.

* **Removing Defaults:** Most modern UI designs (like navbars) start by removing default styling.

<pre>
ul {
  list-style: none; /* Removes bullets */
  padding: 0;       /* Removes default browser indentation */
  margin: 0;
}
</pre>

### 2. Link States (Pseudo-classes)

Links are unique because they have different "states" based on user interaction. To style these, we use **Pseudo-classes**.

Order is critical in CSS (The LVHA rule: Link, Visited, Hover, Active):

`:link:` The default state of an unvisited link.

`:visited:` A link the user has already clicked.

`:hover:` When the user's mouse is over the link.

`:active:` The exact moment the link is being clicked.

`:focus:` When the link is selected via keyboard (crucial for accessibility).

<pre>
  a:link { color: blue; text-decoration: none; }
a:visited { color: purple; }
a:hover { color: red; text-decoration: underline; }
a:active { color: orange; }
</pre>

### Transforming Links into Buttons
By combining the **Box Model** and **Display Models** we previously learned, we can make a simple link look like a professional button.

<pre>
  .nav-button {
  display: inline-block; /* Allows width/height and side-by-side placement */
  padding: 10px 20px;
  background-color: #3498db;
  color: white;
  border-radius: 5px;
  transition: background 0.3s; /* Smooth color change on hover */
}

.nav-button:hover {
  background-color: #2980b9;
}
</pre>

### 📊 Summary of List & Link Properties

| Property | Purpose | Common Values |
| :--- | :---: | :---: |
| `list-style-type` | `Changes/Removes markers.` | `none`, `disc`, `square` |
| `text-decoration` | `Controls underlines on links.` | `none`, `underline` |
| `cursor` | `Changes mouse pointer.` | `pointer`, `default`, `wait` |


-----


### 🧪 Application: The Stylized To-Do List

In your **Stylized To-Do List Lab**, you applied these concepts by:

* Using `list-style: none` to create a clean task container.

* Using `:hover` effects to highlight the task the user is about to select.

* Adding `padding` to list items to make them easier to click on mobile.
