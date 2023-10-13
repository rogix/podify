<script>
	import bgimg from '$lib/images/img-7.jpeg';
	import './styles.css';
</script>

<div class="body">
	<img src={bgimg} alt="bg" />
	<main>
		<slot />
	</main>
</div>

<style>
	.body img {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		object-fit: cover;
		z-index: -1;
	}

	main {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100vh;
	}
</style>
