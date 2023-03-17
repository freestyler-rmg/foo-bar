<template>
	<div>
		<div class="holster mb-24">
			<div class="hihi">Test</div>
		</div>

		<div class="holster holster--sm mb-48">
			<div class="flex mb-24">
				<div class="hihi flex-1">1<br />2<br />3</div>
				<div class="hihi flex-2">2</div>
				<div class="hihi flex-3">3</div>
				<div class="hihi flex-4">4</div>
				<div class="hihi flex-2">2</div>
			</div>
			<div class="flex">
				<div class="hihi flex-3">3</div>
				<div class="hihi flex-3">3</div>
				<div class="hihi flex-3">3</div>
				<div class="hihi flex-3">3</div>
			</div>
		</div>

		<div class="holster holster--md">
			<div class="grid test gap-16 grid-cols-4 md-grid-cols-8 lg-grid-cols-12 mb-24">
				<div class="hihi">1</div>
				<div class="hihi row-start-1 row-end-3 col-start-2">2</div>
				<div class="hihi">3</div>
				<div class="hihi">4</div>
				<div class="hihi col-span-4">5</div>
				<div class="hihi">6</div>
				<div class="hihi">7</div>
				<div class="hihi">8</div>
				<div class="hihi">9</div>
				<div class="hihi">10</div>
				<div class="hihi">11</div>
				<div class="hihi">12</div>
				<div class="hihi">13</div>
				<div class="hihi">14</div>
				<div class="hihi">15</div>
			</div>

			<div class="grid test gap-16 grid-cols-4">
				<div class="hihi">1</div>
				<div class="hihi col-start-1 col-end-2 row-start-1">2 - pulled to position 1</div>
				<div class="hihi">3</div>
				<div class="hihi">4</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'TestingGrid',
}
</script>

<style lang="scss" src="./TestingGrid.scss" scoped />