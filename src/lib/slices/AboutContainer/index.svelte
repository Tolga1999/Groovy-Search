<script>
	/** @type {import("@prismicio/client").Content.AboutContainerSlice} */
	export let slice;
</script>

<section
	class="about-container"
	data-slice-type={slice.slice_type}
	data-slice-variation={slice.variation}
>
<!-- <div class="grain"></div> -->

	<h2>{slice.primary.about_title}</h2>
	<p>{slice.primary.about_text}</p>
	<img src={slice.primary.about_image.url} alt="hot dog gif" />
</section>

<style>
	h2 {
		/* margin-top: 1em;
		margin-bottom: 1em; */
		text-align: left;
		padding: 2rem;
	}

	img {
		width: 100%;
		padding-left: 2rem;
		padding-right: 2rem;
	}

	p {
		text-align: left;
		margin-bottom: 50px;
		padding-left: 2rem;
		padding-right: 2rem;
	}
</style>
