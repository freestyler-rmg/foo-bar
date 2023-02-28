<template>
	<div class="container">
		<section class="mb-16">
			<h2 class="mb-8">
				<code>
					<a href="https://www.w3.org/TR/2011/WD-html5-author-20110809/the-kbd-element.html">
						&lt;kbd&gt;
					</a>
				</code>
			</h2>
			<div>
				<p class="mb-4">No style <kbd>Shift</kbd></p>
				<p>MDN style <kbd class="kbd-mdn">Shift</kbd></p>
			</div>
		</section>

		<hr class="mb-16" />

		<section class="mb-16">
			<h2 class="mb-8">
				<code>
					<a href="https://www.w3.org/TR/2011/WD-html5-author-20110809/the-pre-element.html">&lt;pre&gt;</a>
				</code>
			</h2>
			<div>
				<pre>
       ________________                              _______________
      /                \                            / /           \ \
     / /          \ \   \                          |    -    -       \
     |                  |                          | /        -   \  |
    /                  /                           \                 \
   |      ___\ \| | / /                             \____________  \  \
   |      /           |                             |            \    |
   |      |     __    |                             |             \   \
  /       |       \   |                             |              \  |
  |       |        \  |                             | ====          | |
  |       |       __  |                             | (o-)      _   | |
  |      __\     (_o) |                             /            \  | |
  |     |             |     Heh Heh Heh            /            ) ) | |
   \    ||             \      /      Huh Huh Huh  /             ) / | |
    |   |__             \    /                \  |___            - |  |
    |   |           (*___\  /                  \    *'             |  |
    |   |       _     |    /                    \  |____           |  |
    |   |    //_______|                             ####\          |  |
    |  /       |_|_|_|___/\                        ------          |_/
     \|       \ -         |                        |                |
      |       _----_______/                        \_____           |
      |      /                                          \           |
      |_____/                                            \__________|
				</pre>
			</div>
		</section>

		<hr class="mb-16" />

		<section class="mb-16">
			<h2 class="mb-8">
				<code>
					<a href="https://www.w3.org/TR/2011/WD-html5-author-20110809/the-samp-element.html">
						&lt;samp&gt;
					</a>
				</code>
			</h2>
			<div>
				<p>The computer said <samp>Too much cheese in tray two</samp> but I didn't know what that meant.</p>
			</div>
		</section>

		<hr class="mb-16" />

		<section class="mb-16">
			<h2 class="mb-8">
				<code>
					<a href="https://www.w3.org/TR/2011/WD-html5-author-20110809/the-progress-element.html">
						&lt;progress&gt;
					</a>
				</code>
			</h2>
			<div>
				<p class="mb-4">Progress: <br /><progress max="100" value="50"></progress></p>
				<p class="mb-4">Progress without max: <br /><progress value="0.3"></progress></p>
				<p class="mb-4">Progress without value: <br /><progress max=100></progress></p>
				<p class="mb-4">Progress with <code>accent-color</code>: <br /><progress max="100" value="70" class="progress-accent" /></p>
				<p class="mb-4">Progress with style: <br /><progress max="100" value="70" class="progress-style" /></p>
			</div>
		</section>

		<hr class="mb-16" />

		<section class="mb-16">
			<h2 class="mb-8">
				<code>
					<a href="https://www.w3.org/TR/2011/WD-html5-author-20110809/the-meter-element.html">
						&lt;meter&gt;
					</a>
				</code>
			</h2>
			<div>
				<p class="mb-4">
					Default styling:
					<br />
					<meter min="0" max="100" low="25" high="75" optimum="80" value="10" />
					<br />
					<meter min="0" max="100" low="25" high="75" optimum="80" value="50" />
					<br />
					<meter min="0" max="100" low="25" high="75" optimum="80" value="80" />
					<br />
					<meter min="0" max="100" low="25" high="75" value="30" />
				</p>
				<p class="mb-4">
					Custom styling:
					<br />
					<meter min="0" max="100" low="25" high="75" optimum="80" value="10" class="meter-style" />
				</p>
			</div>
		</section>
	</div>
</template>

<script>
export default {
	name: 'NewHtmlTag',
}
</script>

<style lang="scss" scoped>
a {
	color: #8cb4ff;
}
.kbd-mdn {
	border: 2px solid #696969;
	border-radius: 4px;
	box-shadow: #696969;
	box-shadow: inset 0 -1px 0 0 #696969;
	padding: .25rem;
}

.progress {
	&-accent {
		accent-color: #8a0303;
	}
	&-style {
		appearance: none;
		background-color: #7b5c00;
		box-shadow: inset 1px 1px 5px #8a0303;
		height: 50px;
		width: 250px;
		border-radius: 4px;
		&::-moz-progress-bar,
		&::-webkit-progress-value {
			background-color: #8a0303;
		}
	}
}

.meter-style {
	appearance: none;
	width: 250px;
	height: 50px;
	border: 1px solid #7b5c00;
	border-radius: 8px;
	&::-webkit-meter-bar {
		background: none; /* Required to get rid of the default background property */
		background-color: whiteSmoke;
		box-shadow: 0 5px 5px -5px #333 inset;
	}
	&::-webkit-meter-optimum-value {
		background-color: #f00;
	}
}
</style>