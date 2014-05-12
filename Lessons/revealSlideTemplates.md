#Reveal.JS slide templates

In order to quickly work with reveal.js in creating HTML slide-decks you will need to be familiar with HTML firstly but in order to make it as simple as possible I have included below some HTML slide templates.  All you will need to do is within the `<div class="slides">` section copy in one of the following slide templates including all the tags and example content and then replace the content with your own.

- Title Slide
- Simple slide

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



