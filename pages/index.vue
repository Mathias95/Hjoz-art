<template>
	<div id="home">
		<FrontBanner/>
		<FitfyFiftyLayout/>
		<section class="latest section-padding-lg">
			<div class="container">
				<div class="row justify-content-center"><h2 class="latest__title">Mine seneste malerier</h2></div>
				<div class="row latest__list">
					<LatestCard/>
					<LatestCard/>
					<LatestCard/>
				</div>
				<div class="row justify-content-center">
					<nuxt-link to="" class="btn btn-main">Se flere malerier</nuxt-link>
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