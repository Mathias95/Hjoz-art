<template>
	<div class="work__img-wrapper">
		<div class="work__img-overlay">
			<h3 class="work__img-title text-center">{{ workTitle }}</h3>
		</div>
		<img :src="workImage" alt="" class="work__img">
	</div>	
</template>

<script>
export default {
	props: {
		workImage: {
			type: String,
			required: true
		},
		workTitle: {
			type: String,
			required: true
		},
		id: {
			type: String,
			required: true
		}
	}
}
</script>