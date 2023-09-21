<script>
    	export let data;
</script>

<footer>
	<div class="title">{data.slices[5].primary.footer_title}</div>
	<div class="img">
		<img src={data.slices[5].primary.footer_image.url} alt="" />
	</div>
	<div class="link">
		<a href="{data.slices[5].primary.footer_link.url}">{data.slices[5].primary.footer_link_title}</a>
	</div>
</footer>

<style>
	footer {
		/* position: relative; */
		width: 100%;
		left: 0px;
		bottom: 0;
		padding: 1.2rem 0rem 0rem 1.2rem;
		background-color: rgb(217, 217, 217);
		color: rgb(0, 0, 0);
		margin-top: 70px;
		display: grid;
		grid-template-columns: 0.8fr 1.2fr;
		grid-template-rows: 1fr 1fr;
		grid-auto-columns: 1fr;
		gap: 0px 0px;
		grid-auto-flow: row;
		grid-template-areas: 'title title' 'img link';
	}

	.title {
		font-weight: nomral;
		grid-area: title;
		font-size: 28px;
		width: 75%;
		margin-top: 1rem;
	}

	.img {
		grid-area: img;
		text-align: center;
	}

	.link {
		grid-area: link;
		font-size: 16px;
		margin-top: 2.5rem;
		margin-left: 1.2rem;
	}

	.link a {
		color: rgb(0, 0, 0);
		text-decoration: none;
	}
</style>
