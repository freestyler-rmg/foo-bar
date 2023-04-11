<template>
	<div>
		<div class="holster mb-48">
			<div class="grid grid-cols-3 gap-16 mb-24 mt-16">
				<div>
					<p>width:</p>
					<input id="width" type="number" min="100" max="500" value="250" @input="handleInput">
				</div>
				<div>
					<p>height:</p>
					<input id="height" type="range" min="100" max="500" value="100" @input="handleInput">
				</div>
				<div>
					<p>Color: </p>
					<input id="color" type="color" value="#ff0000" @input="handleInput">
				</div>
			</div>

			<div class="grid">
				<div class="box">
					ballin'
				</div>
			</div>
		</div>

		<div class="holster">
			<div class="grid grid-cols-1 mb-8">
				<div class="mb-16">
					<button class="p-8" @click="toggleTheme">Toggle color</button>
				</div>
				<div class="second-box mb-16" :data-theme="theme">
					<pre>
.second-box {
	$color: #ccc;
	background-color: $color;

	&[data-theme="dark"] {
		$color: #333;
		background-color: $color;
	}
}</pre>
				</div>
				<div class="third-box mb-16" :data-theme="theme">
					<pre>
.third-box {
	--color: #999;
	background-color: var(--color);

	&[data-theme="dark"] {
		--color: #333;
	}
}
</pre>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'CustomProperties',

	data() {
		return {
			theme: 'light',
		}
	},

	methods: {
		handleInput(e) {
			const whichProperty = e.target.id;
			const suffix = e.target.id === 'color' ? '' : 'px';
			const value = e.target.value;
			const box = document.getElementsByClassName('box')[0];
			box.style.setProperty(`--${whichProperty}`, value + suffix);
		},
		toggleTheme() {
			this.theme = this.theme === 'light' ? 'dark' : 'light';
		},
	},
}
</script>

<style lang="scss" scoped src="./CustomProperties.scss" />