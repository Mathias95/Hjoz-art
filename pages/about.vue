<template>
	<div>
		<SubBanner/>
		<section class="section-padding-lg about">
			<div class="container">
				<div class="row align-items-center">
					<div class="col-12 col-md-7 col-lg-6">
						<h2 class="heading-2 about__title">Om Hjoz Art</h2>
						<p class="mb-20 about__subtext">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
						<p class="text-main text-main--dark mb-50 about__maintext">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
						<nuxt-link to="" class="btn btn-main">Kontakt for specialopgaver<i class="material-icons">keyboard_arrow_right</i></nuxt-link>
					</div>
					<div class="col-12 col-md-5 col-lg-6 about__img-wrapper">
						<img src="~assets/images/profile-img.png" alt="" class="about__profile-img">
					</div>
				</div>
			</div>
		</section>
	</div>
</template>

<script>
import SubBanner from '~/components/SubBanner.vue'

export default {
  components: {
    SubBanner
  }
}
</script>