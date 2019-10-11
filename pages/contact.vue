<template>
	<div>
		<SubBanner/>
		<section class="section-padding-lg contact">
			<div class="container">
				<div class="row align-items-center flex-column-reverse flex-md-row">
					<div class="col-12 col-md-5 col-lg-6">
						<img src="~assets/images/contact-img.jpg" alt="" class="contact__img">
					</div>
					<div class="col-12 col-md-7 col-lg-6 contact__col-text">
						<h2 class="heading-2 contact__title">Kontakt</h2>
						<ul class="mb-25 contact__list">
							<span class="contact__name">Heidi Jozwiak</span>
							<li class="contact__item"><i class="material-icons contact__item-icon">room</i><span class="contact__item-info">Adresse:</span>Harrevænget 7, 4200 Slagelse</li>
							<li class="contact__item"><i class="material-icons contact__item-icon">local_phone</i><span class="contact__item-info">Telefon:</span>+45 12 34 56 78</li>
							<li class="contact__item"><i class="material-icons contact__item-icon">mail</i><span class="contact__item-info">Mail:</span>heidi@jozwiak.dk</li>
						</ul>
						<p class="text-main text-main--dark mb-50 contact__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
						<nuxt-link to="" class="btn btn-main">Kontakt for specialopgaver<i class="material-icons">keyboard_arrow_right</i></nuxt-link>
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