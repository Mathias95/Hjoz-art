<template>
	<div>
		<footer class="footer">
			<div class="container">
				<div class="row justify-content-between">
					<div class="col-12 col-lg-6 col-xl-5 mb-50">
						<Logo class="footer__logo mb-25"/>
						<p class="footer__description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco</p>
					</div>
					<div class="col-12 col-lg-5 col-xl-4 mb-40">
						<ul class="footer__contact-list">
							<li class="footer__contact-item">Heidi Jozwiak</li>
							<li class="footer__contact-item"><i class="material-icons footer__contact-icon">room</i><span class="footer__contact-info">Adresse:</span>Harrevænget 6, 4200 Slagelse</li>
							<li class="footer__contact-item"><i class="material-icons footer__contact-icon">local_phone</i><span class="footer__contact-info">Telefon:</span>+45 12 34 56 78</li>
							<li class="footer__contact-item"><i class="material-icons footer__contact-icon">mail</i><span class="footer__contact-info">Mail:</span>heidi@jozwiak.dk</li>
						</ul>
					</div>
				</div>
				<div class="row">
					<div class="col-12">
						<ul class="footer__sitemap">
							<li class="footer__item"><nuxt-link to="/" class="footer__link">Foside</nuxt-link></li>
							<li class="footer__item"><nuxt-link to="/" class="footer__link">Værker</nuxt-link></li>
							<li class="footer__item"><nuxt-link to="/" class="footer__link">Maleri Salg</nuxt-link></li>
							<li class="footer__item"><nuxt-link to="/" class="footer__link">Om Hjoz Art</nuxt-link></li>
							<li class="footer__item"><nuxt-link to="/" class="footer__link">Kontakt</nuxt-link></li>
						</ul>
					</div>
				</div>
			</div>
		</footer>
	</div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>