<script>
	import { SliceZone } from '@prismicio/svelte';
	import { components } from '$lib/slices';

	import Header from '$lib/components/header/+page.svelte'
	import Footer from '$lib/components/footer/+page.svelte'
	
	export let data;
</script>

<Header data={data}/>
<SliceZone slices={data.slices} {components}/>
<Footer data={data}/>
