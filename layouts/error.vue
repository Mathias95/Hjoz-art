<template>
	<section class="section-padding-lg 404">
		<div class="container">
			<div class="row justify-content-center">
				<div class="col-12">
					<img src="~assets/images/404-img.svg" alt="" class="404__img">
				</div>
				<div class="col-12 text-center">
					<nuxt-link to="/" class="404__link btn btn-main">Please return to home<i class="material-icons">keyboard_arrow_right</i></nuxt-link>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	props: {
		error: {
			type: Object,
			default: null
		}
	}

}
</script>

<style>

</style>