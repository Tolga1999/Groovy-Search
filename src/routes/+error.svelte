<script>
  // src/routes/blog/[slug]/+page.svelte
 
  import { page } from '$app/stores';
</script>
 
<h1>{$page.status}: {$page.error?.message}</h1>
<a href="/">Back to Home</a>

<style>
 h1 {
  text-align: center;
  padding: 2rem;
 }

a {
		grid-area: link;
		font-size: 1.5rem;
    text-align: center;
		margin-left: 1.2rem;
		color: rgb(0, 0, 0);
		text-decoration: none;
	}

a:hover {
  cursor: url('/src/lib/assets/CursorSHover.svg'), auto;
}
</style>