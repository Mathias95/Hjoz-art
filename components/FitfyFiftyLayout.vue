<template>
  <section class="fifty">
		<div class="container-fluid">
			<div class="row">
				<div class="col-12 col-lg-6 fifty__img"></div>
				<div class="col-12 col-lg-6 fifty__text-wrapper">
					<h2 class="fifty__title heading-1 mb-30">Lær mere overskrift her</h2>
					<p class="fifty__text text-main text-main--light mb-50">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
					<nuxt-link to="" class="btn btn-main">Se flere malerier<i class="material-icons">keyboard_arrow_right</i></nuxt-link>
				</div>
			</div>
		</div>
  </section>
</template>

<script>
export default {
	props: ['blok']
};
</script>