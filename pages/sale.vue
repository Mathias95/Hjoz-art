<template>
	<div>
		<SubBanner/>
		<section class="sale section-padding-lg">
			<div class="container">
				<div class="row">
					<div class="col-12 col-sm-6 col-lg-4">
						<PaintingSaleCard/>				
					</div>
				</div>
			</div>
		</section>
	</div>
</template>

<script>
import SubBanner from '~/components/SubBanner.vue'
import PaintingSaleCard from '~/components/PaintingSaleCard.vue'

export default {
  components: {
		SubBanner,
		PaintingSaleCard
  }
}
</script>