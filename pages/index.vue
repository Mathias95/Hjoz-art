<template>
	<div id="home">
		<FrontBanner/>
		<FitfyFiftyLayout/>
	</div>
</template>

<script>
import FrontBanner from "~/components/FrontBanner.vue";
import FitfyFiftyLayout from "~/components/FitfyFiftyLayout.vue";
export default {
  components: {
		FrontBanner,
		FitfyFiftyLayout
  }
}
</script>