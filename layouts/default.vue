<template>
  <div>
		<Navigation/>
    <nuxt />
		<section class="bottom-bg">
			This is where the bottom background goes
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