<script lang="ts">
	import Banner from '$lib/Banner.svelte';
	export let data: any = {};
</script>

<svelte:head>
	<title>Marcello Kabora | {data.banner.title} {data.banner.slogan}</title>
</svelte:head>

<Banner {...data.banner} />

<section data-aos="fade-up" data-aos-duration="1000">
	<div class="visual">
		<div class="header">
			<div class="desc">Description</div>
			<div class="date">
				<span>{data.date}</span>
				<span class="material-icons">event</span>
			</div>
		</div>
		<slot />
	</div>
	<div class="header">Gallery</div>
	<div class="gallery">
		{#each data.gallery as photo}
			<div class="photo" data-aos="fade-up" data-aos-duration="1000">
				<img class="image" src={photo} alt="" />
			</div>
		{/each}
	</div>
</section>

<style>
	.header {
		border-bottom: 1px solid silver;
		opacity: 0.5;
		margin-bottom: 20px;
		font-size: 18px;
		display: flex;
		justify-content: space-between;
		padding-top: 40px;
		padding-bottom: 10px;
		font-weight: bold;
	}
	.date {
		display: flex;
		align-items: center;
	}
	.date .material-icons {
		margin-left: 10px;
	}
	.visual {
		flex: 1;
		flex-wrap: wrap;
	}
	.image {
		width: 100% !important;
	}
	.photo {
		position: relative;
		margin-bottom: 20px;
	}
	.photo:hover .image {
		box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
	}
	.image {
		width: 100%;
		transition: all 0.3s;
		box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2);
		border-radius: 3px;
	}
</style>