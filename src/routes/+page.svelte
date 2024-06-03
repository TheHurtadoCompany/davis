<script lang="ts">
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
	import '@splidejs/svelte-splide/css';
</script>

<div class="centered">
	<h1 class="title">Davis</h1>
	<div class="Splide-container">
		<Splide options={{ rewind: true }} aria-label="Svelte Splide Example">
			<SplideSlide>
				<enhanced:img src="/static/hello.jpeg?w=500" alt="puppy" />
			</SplideSlide>
			<SplideSlide>
				<enhanced:img src="/static/sniff.jpeg?w=500" alt="puppy" />
			</SplideSlide>
			<SplideSlide>
				<enhanced:img src="/static/valley.jpeg?w=500" alt="puppy" />
			</SplideSlide>
		</Splide>
	</div>
</div>

<style>
	.centered {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 80vh;
	}
	.Splide-container {
		max-width: 500px;
		margin: 0 auto;
		overflow: hidden;
		border-radius: 20px;
		box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
	}
	.title {
		font-size: 5rem;
		margin-bottom: 1rem;
		font-family:
			system-ui,
			-apple-system,
			BlinkMacSystemFont,
			'Segoe UI',
			Roboto,
			Oxygen,
			Ubuntu,
			Cantarell,
			'Open Sans',
			'Helvetica Neue',
			sans-serif;
	}
</style>
