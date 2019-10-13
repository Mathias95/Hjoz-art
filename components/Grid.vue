<template>
	<section class="section-padding-lg">
		<div class="container">
			<div v-editable="blok" class="row">
				<div class="col-12">
					<h2 class="latest__title heading-1 heading-1--border text-center mx-auto">{{ blok.headline }}</h2>
				</div>
				<component :key="blok._uid" v-for="blok in blok.columns" :blok="blok" :is="blok.component"></component>
			</div>
		</div>
	</section>
</template>

<script>
export default {
  props: ['blok']
}
</script>