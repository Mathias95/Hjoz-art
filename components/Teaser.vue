<template>
	<section class="banner">
		<div class="container">

			<div v-editable="blok" class="row align-items-center">
				<div class="mx-auto col-11 col-md-10 col-lg-5 col-xl-4">
					<h1 class="banner__title">{{ blok.headline }}</h1>
					<p class="banner__text">{{ blok.subtext }}</p>
				</div>

				<div class="col-12 col-lg-7 col-xl-8">
					<div class="banner__right">
						<img :src="image" class="banner__right-img" alt="">
					</div>
				</div>
			</div>

		</div>
	</section>
</template>

<script>
export default {
	computed: {
    image () {
      if (typeof this.blok.image !== 'undefined') {
        return '//img2.storyblok.com/' + this.blok.image.replace('//a.storyblok.com', '')
      }
      return null
    }
  },
  props: ['blok']
}
</script>