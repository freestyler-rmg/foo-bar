.<template>
	<div class="holster">
		<details class="mt-16 mb-24">
			<summary>
				Default Details
			</summary>
			<div class="content">
				Something small enough to escape casual notice.
			</div>
		</details>
		<details class="simple-details mb-24">
			<summary>
				Simple Details
			</summary>
			<div class="content">
				Something small enough to escape casual notice. Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis quam est eum, quasi officia doloribus laborum aliquam laboriosam quia, sit, nisi voluptas architecto nemo iure expedita omnis sed. Quia, a.
			</div>
		</details>
		<details class="bangul-details mb-24">
			<summary>
				BanGul-like Details
			</summary>
			<div class="content">
				The flowing river never stops and yet the water never stays the same.
				<br /><br />
				Foam floats upon the pools, scattering, re-forming, never lingering long.
				<br /><br />
				So it is with man and all his dwelling places here on earth.
			</div>
		</details>
	</div>
</template>

<script lang="ts">
export default {
	name: 'DetailsAccordion',
}
</script>

<style lang="scss" scoped src="./DetailsAccordion.scss">