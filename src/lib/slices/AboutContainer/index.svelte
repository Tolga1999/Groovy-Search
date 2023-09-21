<script>
	/** @type {import("@prismicio/client").Content.AboutContainerSlice} */
	export let slice;
</script>

<section
	class="about-container"
	data-slice-type={slice.slice_type}
	data-slice-variation={slice.variation}
>
	<div class="grain" />
	<!-- Placeholder component for {slice.slice_type} (variation: {slice.variation}) Slices -->

	<h2>{slice.primary.about_title}</h2>
	<p>{slice.primary.about_text}</p>
	<img src={slice.primary.about_image.url} alt="hot dog gif" />
</section>

<style>
	h2 {
		text-align: left;
		padding: 0 2rem;
		margin-top: 1em;
		font-weight: normal;
		margin-bottom: 0.5em;
	}

	img {
		width: 100%;
		padding: 0 2rem;
	}

	p {
		text-align: left;
		margin-bottom: 1.75rem;
		padding: 0 2rem;
	}
</style>
