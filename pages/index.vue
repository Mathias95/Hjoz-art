<template>
	<div id="home">
		<FrontBanner/>
		<FitfyFiftyLayout/>
		<section class="latest section-padding-lg">
			<div class="container">
				<div class="row justify-content-center"><h2>Mine seneste malerier</h2></div>
				<div class="row">
					<div class="col-12 col-md-4"><LatestCard/></div>
					<div class="col-12 col-md-4"><LatestCard/></div>
					<div class="col-12 col-md-4"><LatestCard/></div>
				</div>
				<div class="row justify-content-center">
					<nuxt-link to="">Se flere malerier</nuxt-link>
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