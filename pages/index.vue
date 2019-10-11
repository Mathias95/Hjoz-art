<template>
	<div id="home">
		<FrontBanner/>
		<FitfyFiftyLayout/>
		<section class="latest section-padding-lg">
			<div class="container">
				<div class="row justify-content-center">
					<div class="col">
						<h2 class="latest__title heading-1 heading-1--border text-center mx-auto">Mine seneste malerier</h2>
					</div>
					</div>
				<div class="row flex-wrap latest__list">
					<div class="col-6 col-md-4 latest-card">
						<div class="latest-card__inner">
							<img class="latest-card__img" src="~assets/images/latest-img.jpg" alt="">
						</div>
					</div>
					<div class="col-6 col-md-4 latest-card">
						<div class="latest-card__inner">
							<img class="latest-card__img" src="~assets/images/work-img.jpg" alt="">
						</div>
					</div>
					<div class="col-6 col-md-4 latest-card">
						<div class="latest-card__inner">
							<img class="latest-card__img" src="~assets/images/test-1.jpg" alt="">
						</div>
					</div>
				</div>
				<div class="row justify-content-center">
					<nuxt-link to="" class="btn btn-main">Se flere malerier<i class="material-icons">keyboard_arrow_right</i></nuxt-link>
				</div>
			</div>
		</section>	
	</div>
</template>

<script>
import FrontBanner from "~/components/FrontBanner.vue";
import FitfyFiftyLayout from "~/components/FitfyFiftyLayout.vue";
import LatestCard from "~/components/LatestCard.vue";

export default {
  components: {
		FrontBanner,
		FitfyFiftyLayout,
		LatestCard
  }
}
</script>