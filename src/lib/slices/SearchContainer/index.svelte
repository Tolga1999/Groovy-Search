<script>
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
		margin-top: 3.125em;
	}

	h2 {
		font-size: 1.75em;
		width: 75%;
		font-weight: normal;
	}

	input {
		background-color: white;
		padding: 1.5em 1em;
		border: none;
		border-radius: 1.5em;
		width: 100%;
		margin-top: 1em;
		font-size: 1em;
	}

	input::placeholder {
		padding-left: 0.5em;
		font-size: 1.125em;
	}

	img {
		position: absolute;
		right: 3em;
		transform: translateY(-3.5em);
	}
</style>
