<template>
	<div>
		<SubBanner/>
		<section class="section-padding-lg">
			<div class="container">
				<div class="row justify-content-center">
					<div class="col col-lg-9">
						<h2 class="work__title text-center heading-1 heading-1--border">Udpluk af mine værker</h2>
						<p class="work__text text-center text-main text-main--light mb-80">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit.</p>
					</div>
				</div>
			</div>

			<!--Grid goes here -->
				<div class="container">
					<div class="row">
						<div class="col">
							<WorkCard/>
						</div>
					</div>
				</div>
		</section>	
	</div>
</template>

<script>
import SubBanner from '~/components/SubBanner.vue'
import WorkCard from '~/components/WorkCard.vue'

export default {
  components: {
		SubBanner,
		WorkCard
  }
}
</script>