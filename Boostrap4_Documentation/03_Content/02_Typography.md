

Typography
Documentation and examples for Bootstrap typography, including global settings, headings, body text, lists, and more.

The new generation of project management tools is here and it’s visual.
ads via Carbon
Global settings
Bootstrap sets basic global display, typography, and link styles. When more control is needed, check out the textual utility classes.

Use a native font stack that selects the best font-family for each OS and device.
For a more inclusive and accessible type scale, we assume the browser default root font-size (typically 16px) so visitors can customize their browser defaults as needed.
Use the $font-family-base, $font-size-base, and $line-height-base attributes as our typographic base applied to the <body>.
Set the global link color via $link-color and apply link underlines only on :hover.
Use $body-bg to set a background-color on the <body> (#fff by default).
These styles can be found within _reboot.scss, and the global variables are defined in _variables.scss. Make sure to set $font-size-base in rem.

Headings
All HTML headings, <h1> through <h6>, are available.

Heading	Example
<h1></h1>

h1. Bootstrap heading
<h2></h2>

h2. Bootstrap heading
<h3></h3>

h3. Bootstrap heading
<h4></h4>

h4. Bootstrap heading
<h5></h5>

h5. Bootstrap heading
<h6></h6>

h6. Bootstrap headingCopy
<h1>h1. Bootstrap heading</h1>
<h2>h2. Bootstrap heading</h2>
<h3>h3. Bootstrap heading</h3>
<h4>h4. Bootstrap heading</h4>
<h5>h5. Bootstrap heading</h5>
<h6>h6. Bootstrap heading</h6>
.h1 through .h6 classes are also available, for when you want to match the font styling of a heading but cannot use the associated HTML element.

h1. Bootstrap heading

h2. Bootstrap heading

h3. Bootstrap heading

h4. Bootstrap heading

h5. Bootstrap heading

h6. Bootstrap heading

Copy
<p class="h1">h1. Bootstrap heading</p>
<p class="h2">h2. Bootstrap heading</p>
<p class="h3">h3. Bootstrap heading</p>
<p class="h4">h4. Bootstrap heading</p>
<p class="h5">h5. Bootstrap heading</p>
<p class="h6">h6. Bootstrap heading</p>
Customizing headings
Use the included utility classes to recreate the small secondary heading text from Bootstrap 3.

Fancy display heading With faded secondary text
Copy
<h3>
  Fancy display heading
  <small class="text-muted">With faded secondary text</small>
</h3>
Display headings
Traditional heading elements are designed to work best in the meat of your page content. When you need a heading to stand out, consider using a display heading—a larger, slightly more opinionated heading style.

Display 1
Display 2
Display 3
Display 4Copy
<h1 class="display-1">Display 1</h1>
<h1 class="display-2">Display 2</h1>
<h1 class="display-3">Display 3</h1>
<h1 class="display-4">Display 4</h1>
Lead
Make a paragraph stand out by adding .lead.

Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus.

Copy
<p class="lead">
  Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus.
</p>
Inline text elements
Styling for common inline HTML5 elements.

You can use the mark tag to highlight text.

This line of text is meant to be treated as deleted text.

This line of text is meant to be treated as no longer accurate.

This line of text is meant to be treated as an addition to the document.

This line of text will render as underlined

This line of text is meant to be treated as fine print.

This line rendered as bold text.

This line rendered as italicized text.

Copy
<p>You can use the mark tag to <mark>highlight</mark> text.</p>
<p><del>This line of text is meant to be treated as deleted text.</del></p>
<p><s>This line of text is meant to be treated as no longer accurate.</s></p>
<p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
<p><u>This line of text will render as underlined</u></p>
<p><small>This line of text is meant to be treated as fine print.</small></p>
<p><strong>This line rendered as bold text.</strong></p>
<p><em>This line rendered as italicized text.</em></p>
.mark and .small classes are also available to apply the same styles as <mark> and <small> while avoiding any unwanted semantic implications that the tags would bring.

While not shown above, feel free to use <b> and <i> in HTML5. <b> is meant to highlight words or phrases without conveying additional importance while <i> is mostly for voice, technical terms, etc.

Text utilities
Change text alignment, transform, style, weight, and color with our text utilities and color utilities.

Abbreviations
Stylized implementation of HTML’s <abbr> element for abbreviations and acronyms to show the expanded version on hover. Abbreviations have a default underline and gain a help cursor to provide additional context on hover and to users of assistive technologies.

Add .initialism to an abbreviation for a slightly smaller font-size.

attr

HTML

Copy
<p><abbr title="attribute">attr</abbr></p>
<p><abbr title="HyperText Markup Language" class="initialism">HTML</abbr></p>
Blockquotes
For quoting blocks of content from another source within your document. Wrap <blockquote class="blockquote"> around any HTML as the quote.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

Copy
<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
</blockquote>
Naming a source
Add a <footer class="blockquote-footer"> for identifying the source. Wrap the name of the source work in <cite>.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

Someone famous in Source Title
Copy
<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
Alignment
Use text utilities as needed to change the alignment of your blockquote.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

Someone famous in Source Title
Copy
<blockquote class="blockquote text-center">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

Someone famous in Source Title
Copy
<blockquote class="blockquote text-right">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
Lists
Unstyled
Remove the default list-style and left margin on list items (immediate children only). This only applies to immediate children list items, meaning you will need to add the class for any nested lists as well.

Lorem ipsum dolor sit amet
Consectetur adipiscing elit
Integer molestie lorem at massa
Facilisis in pretium nisl aliquet
Nulla volutpat aliquam velit
Phasellus iaculis neque
Purus sodales ultricies
Vestibulum laoreet porttitor sem
Ac tristique libero volutpat at
Faucibus porta lacus fringilla vel
Aenean sit amet erat nunc
Eget porttitor lorem
Copy
<ul class="list-unstyled">
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>
Inline
Remove a list’s bullets and apply some light margin with a combination of two classes, .list-inline and .list-inline-item.

Lorem ipsum Phasellus iaculis Nulla volutpat
Copy
<ul class="list-inline">
  <li class="list-inline-item">Lorem ipsum</li>
  <li class="list-inline-item">Phasellus iaculis</li>
  <li class="list-inline-item">Nulla volutpat</li>
</ul>
Description list alignment
Align terms and descriptions horizontally by using our grid system’s predefined classes (or semantic mixins). For longer terms, you can optionally add a .text-truncate class to truncate the text with an ellipsis.

Description lists
A description list is perfect for defining terms.
Euismod
Vestibulum id ligula porta felis euismod semper eget lacinia odio sem nec elit.

Donec id elit non mi porta gravida at eget metus.

Malesuada porta
Etiam porta sem malesuada magna mollis euismod.
Truncated term is truncated
Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
Nesting
Nested definition list
Aenean posuere, tortor sed cursus feugiat, nunc augue blandit nunc.
Copy
<dl class="row">
  <dt class="col-sm-3">Description lists</dt>
  <dd class="col-sm-9">A description list is perfect for defining terms.</dd>

  <dt class="col-sm-3">Euismod</dt>
  <dd class="col-sm-9">
    <p>Vestibulum id ligula porta felis euismod semper eget lacinia odio sem nec elit.</p>
    <p>Donec id elit non mi porta gravida at eget metus.</p>
  </dd>

  <dt class="col-sm-3">Malesuada porta</dt>
  <dd class="col-sm-9">Etiam porta sem malesuada magna mollis euismod.</dd>

  <dt class="col-sm-3 text-truncate">Truncated term is truncated</dt>
  <dd class="col-sm-9">Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.</dd>

  <dt class="col-sm-3">Nesting</dt>
  <dd class="col-sm-9">
    <dl class="row">
      <dt class="col-sm-4">Nested definition list</dt>
      <dd class="col-sm-8">Aenean posuere, tortor sed cursus feugiat, nunc augue blandit nunc.</dd>
    </dl>
  </dd>
</dl>
Responsive typography
Responsive typography refers to scaling text and components by simply adjusting the root element’s font-size within a series of media queries. Bootstrap doesn’t do this for you, but it’s fairly easy to add if you need it.

Here’s an example of it in practice. Choose whatever font-sizes and media queries you wish.

Copy
html {
  font-size: 1rem;
}

@include media-breakpoint-up(sm) {
  html {
    font-size: 1.2rem;
  }
}

@include media-breakpoint-up(md) {
  html {
    font-size: 1.4rem;
  }
}

@include media-breakpoint-up(lg) {
  html {
    font-size: 1.6rem;
  }
}
