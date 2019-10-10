<template>
	<div>
		<SubBanner/>
		<section class="sale section-padding-lg">
			<div class="container">
				<div class="row">
					<div class="col-6 col-md-4 sale__card-wrapper">
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