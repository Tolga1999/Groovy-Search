<script>
	export let data;
</script>

<!-- {data.slices[0].primary.logo_title} -->

<section
	class="header"
	data-slice-type={data.slices[0].slice_type}
	data-slice-variation={data.slices[0].variation}
>
	<img src={data.slices[0].primary.logo_image.url} alt="logo" />
	<h2 class="logo">{data.slices[0].primary.logo_title}</h2>
</section>

<style>
	section {
		display: flex;
		align-items: flex-end;
		margin-top: 1.875em;
	}
	img {
		width: 4.5em;
		margin-right: 1em;
	}
	.logo {
		font-size: 1.4em;
		margin-bottom: 0.5em;
	}
</style>
