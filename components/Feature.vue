<template>
	
	<div v-editable="blok" class="col-6 col-md-4 latest-card">
		<h1>{{ blok.name }}</h1>
	</div>
</template>

<script>
export default {
  props: ['blok']
}
</script>