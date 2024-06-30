CSS Notes:
1. Universal Selector:

* {
  color: purple;
}

2. Type Selectors:
<!-- index.html -->

<div>Hello, World!</div>
<div>Hello again!</div>
<p>Hi...</p>
<div>Okay, bye.</div>

/* styles.css */

div {
  color: white;
}


3. Class Selectors:
<!-- index.html -->

<div class="alert-text">Please agree to our terms of service.</div>

/* styles.css */

.alert-text {
  color: red;
}

Another thing you can do with the class attribute is to add multiple classes to a single element as a space-separated list, such as class="alert-text severe-alert".

4. ID Selectors:
<!-- index.html -->

<div id="title">My Awesome 90's Page</div>

/* styles.css */

#title {
  background-color: red;
}

5. Grouping Selectors:
.read,
.unread {
  color: white;
  background-color: black;
}

.read {
  /* several unique declarations */
}

.unread {
  /* several unique declarations */
}

6. Chaining Selectors:
<div>
  <div class="subsection header">Latest Posts</div>
  <p class="subsection preview">This is where a preview for a post might go.</p>
</div>

.subsection.header {
  color: red;
}

This is will only style that has both subsection and header classes. Can be done with classes and id aswell.

7. Descendant combinator:

