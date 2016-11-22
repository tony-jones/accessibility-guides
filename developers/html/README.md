# HTML Guides

*Standards for developing flexible, durable, and sustainable HTML* 

## Table of Contents

  1. [Aria Roles](#aria)
 
### Aria
#### Use [ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) roles appropriately

#### Guidance on using [ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) landmarks

When you use HTML5 sectioning elements it's a good idea to include
the appropriate [ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) landmark roles as well. The trick when you're
using both HTML5 and [ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) is to put the landmark on the sectioning
element itself because this avoids the information being duplicated by
screen readers that support both technologies.

Example:

    <header role="banner"></header>

The following roles map directly to HTML5 sectioning elements:

* `role="main"` maps to the `<main>` element
* `role="complementary"` maps to the `<aside>` element
* `role="contentinfo"` maps to the `<footer>` element
* `role="navigation"` maps to the `<nav>` element

[This article from Léonie Watson](http://tink.uk/screen-readers-aria-roles-html5-support/) explains why using ARIA landmark roles in this way delivers the best experience for screen reader users.

For a more comprehensive guide to the mapping of roles to HTML5 sectioning elements read this [guide](http://blog.paciellogroup.com/2013/02/using-wai-aria-landmarks-2013/) from the Paciello Group.

The following landmark roles don't map to HTML5 elements, but are
still good to use:

* `role="search"`
* `role="application"`

[Demo of how landmark roles help screen reader users](http://tink.co.uk/2011/07/how-do-aria-landmark-roles-help-screen-reader-users/)

#### Main content

The `<main>` tag should be used to identify the main content of your page. Support for it is still marginal so ensure to add the `role="main"` attribute.

#### Sectioned content

When using the `<section>` tag, add an `aria-labelledby` attribute linking to the id of the heading that identifies that section.

Example:

    <section aria-labelledby="advice">
      <h1 id="advice">Help and advice</h1>
