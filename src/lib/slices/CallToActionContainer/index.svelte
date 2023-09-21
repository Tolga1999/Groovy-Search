<script>
	import { PrismicRichText } from '@prismicio/svelte';

	/** @type {import("@prismicio/client").Content.RichTextSlice} */
	export let slice;
</script>

<section class="call-to-action-container" data-slice-type={slice.slice_type} data-slice-variation={slice.variation}>
	<h1 class= first-heading>{slice.primary.call_to_action_heading}</h1>
	<img src={slice.primary.call_to_action_image.url} alt="">
	<button>{slice.primary.search_button}</button>
</section>

<style>
	h1{
		font-size: 2.5em;
		text-align: center;
		margin-top: 50px;
	}

	img{
		width: 100%;
		filter: saturate(0);
		margin-top: 1em;
	}

	button{
		border: none;
		background-color: white;
		font-size: 1em;
		padding: 0.9em 1em;
		border-radius: 1.25em;
		margin-top: 0.8em;
	}
</style>
