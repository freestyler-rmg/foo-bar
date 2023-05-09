.<template>
	<div class="holster">
		<div class="grid grid-cols-2 pt-16">
			<div>
				<div>
					This is 100% HTML font size
				</div>
				<div class="using-px">
					This is 16px
				</div>
				<div class="using-em">
					This is 1em
				</div>
				<div class="using-rem">
					This is 1rem
				</div>
			</div>
			<div>
				<div class="sub-em mb-24">
					This is 0.5em
					<p>
						This child is 2em
					</p>
				</div>
				<div class="sub-rem">
					This is 0.5rem
					<p>
						This child is 2rem
					</p>
				</div>
			</div>
		</div>
	</div>
</template>

<script lang="ts">
export default {
	name: 'FontUnits',
}
</script>

<style lang="scss" scoped src="./FontUnits.scss" />