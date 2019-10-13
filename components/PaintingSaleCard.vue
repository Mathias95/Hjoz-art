<template>
  <div class="painting text-center">
		<div :style="{backgroundImage: 'url(' + thumbnailImage + ')'}" class="painting__img-wrapper mb-20"></div>
		<div class="painting__info">
			<span class="painting__size">{{ sizing }}</span>
			<h3 class="painting__title">{{ title }}</h3>
			<span class="painting__price">{{ pricing }}</span>
		</div>
	</div>
</template>

<script>
export default {
	props: {
		thumbnailImage: {
			type: String,
			required: true
		},
		title: {
			type: String,
			required: true
		},
		sizing: {
			type: String,
			required: true
		},
		pricing: {
			type: String,
			required: true
		},
		id: {
			type: String,
			required: true
		}
	}
};
</script>
