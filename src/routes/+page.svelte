<script>
	import marty from '$lib/assets/marty.jpg';
	
	function routeToBlog() {
		window.location.href = "/Blog";
	}
</script>

<div class="grid-container">
	<div class="box">
		<h1>
		Welcome to harrywitt.org!
		</h1>
		<p>
		My name is Harry Witt. I'm a Software Engineer passionate about the command line, taking the path of most resistance, football, cinema, and music. In my free time, I like to lift weights, read, watch movies, and argue with people on the internet.
		</p>
		<img src={marty} alt="Image" />
		<button on:click={() => {routeToBlog()}}>
			Blog
		</button>
	</div>
</div>

<style>
	:global(body) {
		font-family: 'Fira Code', monsopace;
		margin: 0;
		background-color: black;
		color: white;
	}
	.grid-container {
		display: grid;
		place-items: center;
		height: 0vh;
	}
	.box {
		padding: 3rem;
	}
	h1 {
		font-weight: bold;
		font-size: 35px;
		margin-bottom: 2rem;
	}
	p {
		margin-bottom: 2rem;
	}
	img {
		margin-bottom: 2rem;
	}
	button {
		color: blue;
	}
</style>
