<script>
	/** @type {import("@prismicio/client").Content.SearchContainerSlice} */
	export let slice;
</script>

<section
	class="search-container"
	data-slice-type={slice.slice_type}
	data-slice-variation={slice.variation}
>
	<form>
		<h2>{slice.primary.search_title}</h2>
		<input type="text" placeholder={slice.primary.input_placeholder} />
		<img src={slice.primary.input_svg.url} alt="" />
	</form>
</section>

<style>
	section {
		/* position: relative; */
		margin-top: 3.125em;
	}

	h2 {
		font-weight: normal;
		font-size: 1.75em;
		width: 75%;
	}

	input {
		background-color: white;
		padding: 1.5em 1em;
		border: none;
		border-radius: 1.5em;
		width: 100%;
		max-width: 30em;
		margin-top: 1em;
		font-size: 1em;
		z-index: 2;
	}

	input::placeholder {
		padding-left: 0.5em;
		font-size: 1.125em;
	}

	img {
		position: absolute;
		right: 3em;
		transform: translateY(-3.5em);
		z-index: 3;
	}

	input, input::placeholder{
		position: relative;
	}

	@media (min-width: 700px) {
		img {
			display: none;
		}
	}
</style>
