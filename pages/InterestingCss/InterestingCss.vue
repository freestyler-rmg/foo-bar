.<template>
	<div class="holster">
		<h2 class="mt-16 mb-16">CSS Property</h2>
		<div class="grid grid-cols-2 gap-16">
			<div class="mb-16">
				<h4 class="mb-8">
					<code>contain</code>
				</h4>
				<div class="contain-example contain-fixed mb-8">
					position relative with contain layout
					<br />
					Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis, laudantium consequatur nostrum velit consectetur natus id quidem nam esse nobis impedit aliquam odio, ipsa reiciendis officia quos neque, ipsam sapiente accusamus. Fugiat sequi architecto, molestiae adipisci dicta illum dolore laudantium odit quisquam non alias ullam voluptatum obcaecati nobis unde, quas delectus placeat iusto accusantium deleniti vitae hic odio aut. Facere delectus inventore aliquid dolor illo sequi! Inventore harum excepturi sed eos vero mollitia eum perspiciatis a! Vero tenetur perspiciatis explicabo! Necessitatibus eveniet doloremque illo perferendis fugiat? Consequuntur nisi optio voluptatum mollitia sint, tenetur quae recusandae alias quisquam! Eligendi, possimus est.

					<div class="fixed">
						position fixed, bottom 0, right 0
					</div>
				</div>

				<div class="contain-example contain-layout">
					some text before float
					<p class="float-left">
						float left text
						<img src="https://picsum.photos/seed/picsum/200/300" alt="">
					</p>
				</div>
			</div>

			<div class="mb-16">
				<h4 class="mb-8">
					<code>inset</code>
				</h4>

				<div class="inset-testing">
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui suscipit corrupti, incidunt sit enim harum optio sunt ex, quos assumenda vel, veniam consectetur corporis! Natus magnam quod impedit cumque in!
					<div class="child">
						position absolute
					</div>
				</div>
			</div>
		</div>

		<hr />

		<h2 class="mt-16 mb-16">CSS Pseudo-element</h2>
		<div class="grid grid-cols-2 gap-16">
			<div class="mb-16">
				<h4 class="mb-8">
					<code>::file-selector-button</code>
				</h4>

				<div class="file-selector-button">
					<input type="file">
				</div>
			</div>

			<div class="mb-16">
				<h4 class="mb-8">
					<code>::selection</code>
				</h4>

				<div class="text-selection">
					Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsam dicta, laboriosam quis sapiente repudiandae voluptatum sint nobis cupiditate, libero iure eligendi dignissimos aliquam sit quidem provident illo, nesciunt quibusdam. Incidunt!
				</div>
			</div>
		</div>

		<hr />

		<h2 class="mt-16 mb-16">CSS Pseudo-class</h2>
		<div class="grid grid-cols-2 gap-16">

			<div class="mb-16">
				<h4 class="mb-8">
					<code>:has</code>
				</h4>

				<div class="foo">
					<div class="bar">
						foo bar
					</div>
				</div>
			</div>

			<div class="mb-16">
				<h4 class="mb-8">
					<code>:is()</code> and <code>:where()</code>
				</h4>

				<div class="is-where-styling">
					<div class="is-styling">
						<p>is styling - I should be red</p>
					</div>
					<div class="where-styling">
						<p>where styling - I'm blue but getting override by green "p" styling</p>
					</div>
				</div>
			</div>

			<div class="mb-16">
				<h4 class="mb-8">
					<code>:placeholder-shown</code>
				</h4>

				<div class="placeholder-styling mb-8">
					<input type="text" placeholder="placeholder">
				</div>

				<div class="placeholder-shown-styling">
					<input type="text" placeholder="placeholder-shown">
				</div>

			</div>
		</div>
	</div>
</template>

<script lang="ts">
export default {
	name: 'InterestingCss',
}
</script>

<style lang="scss" scoped src="./InterestingCss.scss" />