<script>
	import { Parallax, ParallaxLayer } from 'svelte-parallax'
	import Banner from './Banner.svelte'
	import CarrouselIndustries from './Banner_with_Carrousel.svelte'

	let parallax

	const url = (name, wrap = false) =>
		`${wrap ? 'url(' : ''}https://awv3node-homepage.surge.sh/build/assets/${name}.svg${wrap ? ')' : ''}`
</script>

<Parallax sections="2" bind:this={parallax}>
	<ParallaxLayer
		offset="0"
		rate="0"
		span="2"
		style="background-image: {url('stars', true)}; background-size: cover;"
	/>

	<ParallaxLayer offset="0.8" rate="-0.3" style="opacity: 0.3;">
		<img src="/parallax/wine-opener-svgrepo-com.svg" alt="" style="display: block; width: 10%; margin-left: 55%;" />
	</ParallaxLayer>

	<ParallaxLayer offset="0.0" rate="0.2" style="opacity: 0.1;">
		<img src="/parallax/wine-glass-svgrepo-com.svg" alt="" style="display: block; width: 10%; margin-left: 55%;" />
	</ParallaxLayer>
	<ParallaxLayer offset="0.2" rate="0.8" style="opacity: 0.1;">
		<img
			src="/parallax/wine-svgrepo-com.svg"
			alt=""
			style="display: block; width: 10%; margin-left: 15%;"
		/>
	</ParallaxLayer>

	<ParallaxLayer offset="0.75" rate="0.5" style="opacity: 0.1;">
		<img
			src="/parallax/wine-barrel-svgrepo-com.svg"
			alt=""
			style="display: block; width: 10%; margin-left: 70%;"
		/>
		<img src="/parallax/wine-svgrepo-com-2.svg" alt="" style="display: block; width: 10%; margin-left: 40%;" />
	</ParallaxLayer>

	<ParallaxLayer offset="0" rate="0.2" style="opacity: 0.1;">
		<img src="/parallax/the-trees-svgrepo-com.svg" alt="" style="display: block; width: 10%; margin-left: 10%;" />
		<img src="/parallax/the-trees-svgrepo-com.svg" alt="" style="display: block; width: 10%; margin-left: 75%;" />
	</ParallaxLayer>

	<ParallaxLayer offset="0.6" rate="-0.1" style="opacity: 0.1;">
		<img src="/parallax/indicator-svgrepo-com.svg" alt="" style="display: block; width: 10%; margin-left: 60%;" />
		<img src="/parallax/map-svgrepo-com.svg" alt="" style="display: block; width: 10%; margin-left: 30%;" />
	</ParallaxLayer>

	<ParallaxLayer
		offset="1.4"
		rate="-0.4"
		style="display: flex; align-items: center; justify-content: center;"
	>
		<img src="/parallax/wine-svgrepo-com-2.svg	" alt="" style="width: 60%;" />
	</ParallaxLayer>

	<ParallaxLayer
		offset="0"
		rate="0.1"
		style="display: flex; align-items: center; justify-content: center;"
	>
		<Banner></Banner>
	</ParallaxLayer>
</Parallax>

<style>
	:global(body) {
		padding: 0;
	}
	img:focus {
		outline: 1px dotted gray;
	}
	img:focus:not(:focus-visible) {
		outline: none;
	}
</style>
