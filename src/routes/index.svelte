<script context="module">
	import Munchi from '$lib/components/Munchi.svelte';
	export const prerender = true
</script>

<script>
	import { Swipe, SwipeItem } from "svelte-swipe";
	const swipeConfig = {
	autoplay: true,
	delay: 10000,
	showIndicators: false,
	transitionDuration: 333,
	defaultIndex: 0,
};
</script>

<svelte:head>
	<title>Leonela Venturo | Copywriter & Seo</title>
</svelte:head>

<main>
		<Swipe {...swipeConfig}>
		  <SwipeItem>
			<Munchi />
		  </SwipeItem>
	  
		  <SwipeItem>

		  </SwipeItem>
	  
		  <SwipeItem>
			<Munchi />
		  </SwipeItem>
		</Swipe>



	<!-- <div class="container">
		<h2>Contando tu historia en vez de un simple “sobre&nbsp;mi”, lograrás sobresalir entre otras personas que copian y pegan sus objetivos.</h2>
	</div> --> 
</main>

<style>
main{
	height: 100vh;
    width: 100%;
	position: absolute;
	bottom: 0;
	z-index: 1;
	padding-top: 80px;
	display:flex;
	justify-content: center;
	flex-direction: column;
	align-items: center;
}
main .container{
	color: white;
	position: absolute;
	bottom: 0;
	display: flex;
	justify-content: center;
	margin: 0 0 3em 0;
	z-index: 2;
	backdrop-filter: blur(4px);
	background: rgba(80, 54, 73, 0.3);
}
h2{
	text-align: center;
	padding: 0 20px;
	font-size: 0.9rem;
	letter-spacing: 1.4px;
	line-height: 27px;
	text-transform: uppercase;
	font-family: Poppins;
	font-style: normal;
	font-weight: normal;
	text-align: center;
	font-variant: small-caps;
	text-shadow: 1px 1px 1px rgba(66, 20, 60, 0.8);
	color: #FFFFFF;
}
</style>
