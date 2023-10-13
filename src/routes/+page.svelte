<script>
	import img1 from '$lib/images/img-1.jpeg';
	import img2 from '$lib/images/img-2.jpeg';
	import img3 from '$lib/images/img-3.jpeg';
	import img4 from '$lib/images/img-4.jpeg';
	import img5 from '$lib/images/img-5.jpeg';
	import img6 from '$lib/images/img-6.jpeg';
	import img7 from '$lib/images/img-7.jpeg';

	import volume from '$lib/icons/volume.svg';
	import foward from '$lib/icons/foward.svg';
	import backward from '$lib/icons/backward.svg';
	import pause from '$lib/icons/pause.svg';
</script>

<div class="wrapper">
	<div class="search">
		<input type="text" placeholder="Buscar" />
	</div>

	<section class="glass-section">
		<aside class="genres">
			<h2>podfy</h2>

			<nav>
				<ul>
					<li class="active">Todos</li>
					<li>Histórias</li>
					<li>Comédia</li>
					<li>Notícias</li>
					<li>Esportes</li>
					<li>Política</li>
					<li>Religião</li>
					<li>Entretenimento</li>
					<li>Outros</li>
				</ul>
			</nav>
		</aside>
		<div class="list">
			<article>
				<img src={img1} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
			<article>
				<img src={img4} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
			<article>
				<img src={img3} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
			<article>
				<img src={img2} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
			<article>
				<img src={img5} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
			<article>
				<img src={img6} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
			<article>
				<img src={img7} alt="img1" />
				<div class="info">
					<h2>Mano a Mano</h2>
					<p>Spotify Studios</p>
				</div>
			</article>
		</div>
	</section>

	<div class="player">
		<div class="player__img">
			<img src={volume} alt="img1" />
		</div>
		<div class="player__info">
			<h2>Djamila Ribeiro</h2>
		</div>
		<div class="player__controls">
			<button class="player__controls--prev">
				<img src={backward} alt="backward" />
			</button>
			<button class="player__controls--play">
				<img src={pause} alt="pause" />
			</button>
			<button class="player__controls--next">
				<img src={foward} alt="foward" />
			</button>
		</div>
	</div>
</div>

<style>
	.wrapper {
		display: flex;
		flex-direction: column;
		align-items: center;
		height: 95%;
	}

	.search {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 50%;
		height: 10%;
		margin-bottom: 1rem;
		background: rgba(37, 35, 35, 0.5);
		backdrop-filter: blur(10px);
		border-radius: 40px;
	}

	.search input {
		width: 95%;
		height: 60%;
		border: none;
		background: rgba(35, 35, 35, 0.5);
		padding: 0 1rem;
		font-size: 1rem;
		color: #fff;
		border-radius: 40px;
	}

	.glass-section {
		display: flex;
		height: 70%;
		width: 70%;
		background: rgba(35, 35, 35, 0.5);
		backdrop-filter: blur(10px);
		border-radius: 40px;
		padding: 1rem;
		overflow: auto;
	}

	.glass-section .list {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		gap: 1rem;
		margin-inline: 30px;
		/* width: 100%; */
	}

	.glass-section article {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		background: rgba(37, 35, 35, 0.5);
		backdrop-filter: blur(10px);
		border-radius: 10px;
		padding: 1rem;
		background: rgba(37, 35, 35, 0.5);
		box-shadow: inset 3px 3px 3px rgb(36 36 36 / 40%), inset -3px -3px 3px #282828;
	}

	.glass-section article img {
		max-width: 100%;
		width: auto;
		height: 100%;
		object-fit: cover;
		border-radius: 10px;
	}

	.glass-section .genres {
		width: 30%;
		display: flex;
		flex-direction: column;
		gap: 1rem;
		justify-content: center;
		border-radius: 10px;
		padding: 1rem;
		margin-right: 30px;
		padding-top: 50px;
	}

	.glass-section .genres h2 {
		font-size: 2rem;
		margin-bottom: 1rem;
		color: #fff;
	}

	.glass-section .genres nav ul {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}

	.glass-section .genres nav li {
		color: #9f9f9f;
		padding: 10px;
		border-radius: 10px;
	}

	.glass-section .genres nav li:hover,
	.glass-section .genres nav li.active {
		cursor: pointer;
		color: #fff;
		background: rgba(35, 35, 35, 0.5);
		box-shadow: inset 3px 3px 3px #353535, inset -3px -3px 3px #353535;
	}

	.info {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
		margin-top: 1rem;
		gap: 1rem;
		width: 100%;
	}

	.info h2 {
		font-size: 1rem;
		color: #fff;
	}

	.info p {
		font-size: 1rem;
		color: #9f9f9f;
	}

	.player {
		display: flex;
		align-items: center;
		justify-content: space-between;
		width: 30%;
		height: 60px;
		margin-block-start: 20px;
		background: rgba(37, 35, 35, 0.5);
		backdrop-filter: blur(10px);
		border-radius: 40px;
		padding: 1rem;
	}

	.player__info {
		display: flex;
		background-color: rgba(35, 35, 35, 0.1);
		backdrop-filter: blur(10px);
		border-radius: 40px;
		padding: 0.75rem;
		width: 70%;
		gap: 0.5rem;
		color: #fff;
	}

	.player__controls button {
		background-color: transparent;
		border: none;
		color: #fff;
	}

	.player__controls img {
		color: #fff;
	}
</style>
