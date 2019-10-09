<template>
	<div>
		<nav class="nav">
			<div class="container nav__wrapper">
				<div class="nav__brand">
					<logo/>
					<button class="nav__hamburger">
						<span class="nav__line"></span>
						<span class="nav__line"></span>
						<span class="nav__line"></span>
					</button>
				</div>
				<div class="nav__menu">
					<ul class="nav__list">
						<li class="nav__item"><nuxt-link to="/" class="nav__link">Forside</nuxt-link></li>
						<li class="nav__item"><nuxt-link to="/work" class="nav__link">Værker</nuxt-link></li>
						<li class="nav__item"><nuxt-link to="/sale" class="nav__link">Maleri Salg</nuxt-link></li>
						<li class="nav__item"><nuxt-link to="/about" class="nav__link">Om Hjoz Art</nuxt-link></li>
						<li class="nav__item"><nuxt-link to="/contact" class="nav__link">Kontakt</nuxt-link></li>
					</ul>
				</div>
			</div>
		</nav>
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