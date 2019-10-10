<template>
  <div class="site">
		<Navigation/>
    <nuxt/>
		<section class="bottom">
			<div class="bottom__bg"></div>
		</section>
		<BackTop/>
		<Footer/>
  </div>
</template>

<script>
import Navigation from "~/components/Navigation.vue";
import BackTop from "~/components/BackTop.vue";
import Footer from "~/components/Footer.vue";

export default {
	components: {
		Navigation,
		BackTop,
		Footer
	}
}
</script>