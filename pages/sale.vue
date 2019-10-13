<template>
	<div>
		<SubBanner/>
		<section class="sale section-padding-lg">
			<div class="container">
				<div class="row">
					<div class="col-6 col-md-4 sale__card-wrapper" v-for="sale in sales" 
						:key="sale.id">
						<PaintingSaleCard
						:thumbnailImage="sale.thumbimage"
						:sizing="sale.size"
						:title="sale.title"
						:pricing="sale.price"
						:id="sale.id"/>
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
	},
	asyncData(context) {
		return context.app.$storyapi.get('cdn/stories', {
			version: 'draft',
			starts_with: 'sale/'
		}).then(res => {
			//console.log(res);
			
			return {
				sales: res.data.stories.map(bp => {
					return {
						id: bp.slug,
						title: bp.content.title,
						size: bp.content.size,
						price: bp.content.price,
						thumbimage: bp.content.image
					}
				})
			};
		});
	}
	// data() {
	// 	return {
	// 		sales: [
	// 			{
	// 				size: "40x50 cm",
	// 				title: "Udvalg af maleri 1",
	// 				price: "Pris pr. stk. 800,-",
	// 				thumbimage: "https://images.unsplash.com/photo-1541753866388-0b3c701627d3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80",
	// 				id: "first-sale"
	// 			},
	// 			{
	// 				size: "40x50",
	// 				title: "Udvalg af maleri 2",
	// 				price: "Pris pr. stk. 800,-",
	// 				thumbimage: "https://images.unsplash.com/photo-1541753866388-0b3c701627d3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80",
	// 				id: "second-sale"
	// 			}
	// 		]
	// 	}
	// }
}
</script>