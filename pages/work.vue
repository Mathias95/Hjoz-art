<template>
	<div>
		<SubBanner/>
		<section class="section-padding-lg">
			<div class="container">
				<div class="row justify-content-center">
					<div class="col col-lg-9">
						<h2 class="work__title text-center heading-1 heading-1--border mx-auto">Udpluk af mine værker</h2>
						<p class="work__text text-center text-main text-main--light mb-80">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit.</p>
					</div>
				</div>
			</div>

			<!--Grid goes here -->
			<div class="container">
				<div class="row">
					<div class="work__grid">
						<div class="col-12" 
						v-for="work in works"
						:key="work.id">
							<WorkCard
							:workImage="work.paintImg"
							:workTitle="work.title"
							:id="work.id"/>
						</div>
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
	},
	data(){
		return {
			works: [
				{
					title: "Navn på maleri 1",
					paintImg: "https://images.unsplash.com/photo-1570964249954-e387322dd586?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=701&q=80",
					id: "one-paint"
				},
				{
					title: "Navn på maleri 2",
					paintImg: "https://images.unsplash.com/photo-1570948510276-aea76a9a4391?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80",
					id: "two-paint"
				},
				{
					title: "Navn på maleri 3",
					paintImg: "https://images.unsplash.com/photo-1569286122346-2a0cef3e7ad8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=675&q=80",
					id: "three-paint"
				},
				{
					title: "Navn på maleri 4",
					paintImg: "https://images.unsplash.com/photo-1570937937487-125575170d69?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80",
					id: "four-paint"
				},
				{
					title: "Navn på maleri 5",
					paintImg: "https://images.unsplash.com/photo-1558981285-501cd9af9426?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80",
					id: "five-paint"
				},
				{
					title: "Navn på maleri 6",
					paintImg: "https://images.unsplash.com/photo-1570821806133-55200c3adde3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80",
					id: "six-paint"
				},
				{
					title: "Navn på maleri 7",
					paintImg: "https://images.unsplash.com/photo-1556909172-89cf0b24ff02?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1351&q=80",
					id: "seven-paint"
				}
			]
		}
	}
}
</script>