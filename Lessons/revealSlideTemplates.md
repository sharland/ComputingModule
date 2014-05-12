#Reveal.JS slide templates

In order to quickly work with reveal.js in creating HTML slide-decks you will need to be familiar with HTML firstly but in order to make it as simple as possible I have included below some HTML slide templates.  All you will need to do is within the `<div class="slides">` section copy in one of the following slide templates including all the tags and example content and then replace the content with your own.

- [Title Slide](https://github.com/sharland/ComputingModule/blob/master/Lessons/revealSlideTemplates.md#title-slide)
- [Simple slide](#simple-slide)

##Title Slide
```html
			<section>
				<h1>Reveal.js</h1>
				<h3>HTML Presentations Made Easy</h3>
					<p>
					<small>Created by <a href="http://hakim.se">Hakim El Hattab</a> / <a href="http://twitter.com/hakimel">@hakimel</a></small>
					</p>
			</section>
```

##Simple Slide
Showing the use of speaker notes using `<aside class="notes">`
```html
			<section>
				<h2>Heads Up</h2>
					<p>reveal.js is a framework for easily creating beautiful presentations using HTML. You'll need a browser with support for CSS 3D transforms to see it in its full glory.</p>

				<aside class="notes">Oh hey, these are some notes. They'll be hidden in your presentation, but you can see them if you open the speaker notes window (hit 's' on your keyboard).</aside>
				</section>
```

##Nested vertical slides
Note how `<section>` is nested to provide the vertical slides. Images have also been inserted.
```html
				<section>
					<section>
						<h2>Vertical Slides</h2>
						<p>
							Slides can be nested inside of other slides,
							try pressing <a href="#" class="navigate-down">down</a>.
						</p>
						<a href="#" class="image navigate-down">
							<img width="178" height="238" src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Down arrow">
						</a>
					</section>
					<section>
						<h2>Basement Level 1</h2>
						<p>Press down or up to navigate.</p>
					</section>
					<section>
						<h2>Basement Level 2</h2>
						<p>Cornify</p>
						<a class="test" href="http://cornify.com">
							<img width="280" height="326" src="https://s3.amazonaws.com/hakim-static/reveal-js/cornify.gif" alt="Unicorn">
						</a>
					</section>
					<section>
						<h2>Basement Level 3</h2>
						<p>That's it, time to go back up.</p>
						<a href="#/2" class="image">
							<img width="178" height="238" src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Up arrow" style="-webkit-transform: rotate(180deg);">
						</a>
					</section>
				</section>
```
##Unordered list
```html
				<section>
					<h2>Marvelous Unordered List</h2>
					<ul>
						<li>No order here</li>
						<li>Or here</li>
						<li>Or here</li>
						<li>Or here</li>
					</ul>
				</section>
```

##Ordered list
```html
				<section>
					<h2>Fantastic Ordered List</h2>
					<ol>
						<li>One is smaller than...</li>
						<li>Two is smaller than...</li>
						<li>Three!</li>
					</ol>
				</section>
```html

##Slide with own background colour
```html
					<section data-background="#007777">
						<h2>Slide Backgrounds</h2>
						<p>
							Set <code>data-background="#007777"</code> on a slide to change the full page background to the given color. All CSS color formats are supported.
						</p>
						<a href="#" class="image navigate-down">
							<img width="178" height="238" src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Down arrow">
						</a>
					</section>
```

##Slide with image background
```html
					<section data-background="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png">
						<h2>Image Backgrounds</h2>
						<pre><code>&lt;section data-background="image.png"&gt;</code></pre>
					</section>
```

##Slide with repeating image background
```html
					<section data-background="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" data-background-repeat="repeat" data-background-size="100px">
						<h2>Repeated Image Backgrounds</h2>
						<pre><code style="word-wrap: break-word;">&lt;section data-background="image.png" data-background-repeat="repeat" data-background-size="100px"&gt;</code></pre>
					</section>
```
##Code block
```html
					<section>
						<h2>Example Code</h2>
						<pre><code style="word-wrap: break-word;">&lt;section data-background="image.png" data-background-repeat="repeat" data-background-size="100px"&gt;</code></pre>
					</section>
```

##Another code block example
```html
				<section>
					<h2>Pretty Code</h2>
					<pre><code data-trim contenteditable>
function linkify( selector ) {
  if( supports3DTransforms ) {

    var nodes = document.querySelectorAll( selector );

    for( var i = 0, len = nodes.length; i &lt; len; i++ ) {
      var node = nodes[i];

      if( !node.className ) {
        node.className += ' roll';
      }
    }
  }
}
					</code></pre>
					<p>Courtesy of <a href="http://softwaremaniacs.org/soft/highlight/en/description/">highlight.js</a>.</p>
				</section>
```

##Putting quotes in
```html
				<section>
					<h2>Clever Quotes</h2>
					<p>
						These guys come in two forms, inline: <q cite="http://searchservervirtualization.techtarget.com/definition/Our-Favorite-Technology-Quotations">
						&ldquo;The nice thing about standards is that there are so many to choose from&rdquo;</q> and block:
					</p>
					<blockquote cite="http://searchservervirtualization.techtarget.com/definition/Our-Favorite-Technology-Quotations">
						&ldquo;For years there has been a theory that millions of monkeys typing at random on millions of typewriters would
						reproduce the entire works of Shakespeare. The Internet has proven this theory to be untrue.&rdquo;
					</blockquote>
				</section>
```

##Linking between slides
```html
				<section>
					<h2>Intergalactic Interconnections</h2>
					<p>
						You can link between slides internally,
						<a href="#/2/3">like this</a>.
					</p>
				</section>
```

##Simple content animation
```html
				<section>
					<section id="fragments">
						<h2>Fragmented Views</h2>
						<p>Hit the next arrow...</p>
						<p class="fragment">... to step through ...</p>
						<ol>
							<li class="fragment"><code>any type</code></li>
							<li class="fragment"><em>of view</em></li>
							<li class="fragment"><strong>fragments</strong></li>
						</ol>

						<aside class="notes">
							This slide has fragments which are also stepped through in the notes window.
						</aside>
					</section>
```

##Fancier content animation
```html
					<section>
						<h2>Fragment Styles</h2>
						<p>There's a few styles of fragments, like:</p>
						<p class="fragment grow">grow</p>
						<p class="fragment shrink">shrink</p>
						<p class="fragment roll-in">roll-in</p>
						<p class="fragment fade-out">fade-out</p>
						<p class="fragment highlight-red">highlight-red</p>
						<p class="fragment highlight-green">highlight-green</p>
						<p class="fragment highlight-blue">highlight-blue</p>
						<p class="fragment current-visible">current-visible</p>
						<p class="fragment highlight-current-blue">highlight-current-blue</p>
					</section>
```
##Example image with link
```html
				<section>
					<h2>Spectacular image!</h2>
					<a class="image" href="http://lab.hakim.se/meny/" target="_blank">
						<img width="320" height="299" src="http://s3.amazonaws.com/hakim-static/portfolio/images/meny.png" alt="Meny">
					</a>
				</section>
```



