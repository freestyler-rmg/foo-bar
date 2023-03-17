<template>
	<div>
		<div class="holster pt-24">

			<div class="slider-holster">
				<div class="slider-container">
					<div class="sliders">
						<div id="slide-a" class="slider-item">
							A
							<nav class="slider-prev-next">
								<div>
									<a href="#slide-e">prev</a>
									<a href="#slide-b">next</a>
								</div>
							</nav>
						</div>
						<div id="slide-b" class="slider-item">
							B
							<nav class="slider-prev-next">
								<div>
									<a href="#slide-a">prev</a>
									<a href="#slide-c">next</a>
								</div>
							</nav>
						</div>
						<div id="slide-c" class="slider-item">
							C
							<nav class="slider-prev-next">
								<div>
									<a href="#slide-b">prev</a>
									<a href="#slide-d">next</a>
								</div>
							</nav>
						</div>
						<div id="slide-d" class="slider-item">
							D
							<nav class="slider-prev-next">
								<div>
									<a href="#slide-c">prev</a>
									<a href="#slide-e">next</a>
								</div>
							</nav>
						</div>
						<div id="slide-e" class="slider-item">
							E
							<nav class="slider-prev-next">
								<div>
									<a href="#slide-d">prev</a>
									<a href="#slide-a">next</a>
								</div>
							</nav>
						</div>
					</div>

					<div class="nav-faker">
						<div>prev button</div>
						<div>next button</div>
					</div>
				</div>

				<nav class="slider-link">
					<a href="#slide-a">A</a>
					<a href="#slide-b">B</a>
					<a href="#slide-c">C</a>
					<a href="#slide-d">D</a>
					<a href="#slide-e">E</a>
				</nav>
			</div>

		</div>
	</div>
</template>

<script lang="ts">
export default {
	name: 'SliderTesting',
}
</script>

<style lang="scss" scoped src="./SliderTesting.scss" />