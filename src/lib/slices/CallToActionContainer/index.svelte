<script>
	import { PrismicRichText } from '@prismicio/svelte';

	/** @type {import("@prismicio/client").Content.RichTextSlice} */
	export let slice;
</script>

<section
	class="call-to-action-container"
	data-slice-type={slice.slice_type}
	data-slice-variation={slice.variation}
>
	<h1 class="first-heading">{slice.primary.call_to_action_heading}</h1>
	<div class="image-button-container">
		<img src={slice.primary.call_to_action_image.url} alt="" />
		<button><a href="#all-members">{slice.primary.search_button}</a></button>
	</div>
</section>

<style>
	h1 {
		font-weight: normal;
		font-size: 2.5em;
		text-align: center;
		margin-top: 50px;
	}

	img {
		width: 100%;
		max-width: 37.5em;
		filter: saturate(0);
		margin-top: 1em;
		position: relative;
		z-index: 2;
	}

	button {
		border: none;
		background-color: white;
		font-size: 1em;
		padding: 0.9em 1em;
		border-radius: 1.25em;
		margin-top: 0.8em;
	}

	button a {
		text-decoration: none;
		color: black;
	}

	/* media queries for desktop */
	@media (min-width: 700px) {
		section {
			display: flex;
			flex-direction: column;
			align-items: center;
		}

		h1 {
			display: flex;
			justify-content: flex-start;
		}
	}
</style>
