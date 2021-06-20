<script context="module">
	import Munchi from '$lib/components/Munchi.svelte';
	export const prerender = true
</script>

<script>
	import { Swipe, SwipeItem } from "svelte-swipe";
	const swipeConfig = {
	autoplay: false,
	delay: 15000,
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
		  <SwipeItem class="swipeContainer">
			  <p class="text">
				Compartir buen contenido es un desafío si no tienes las herramientas para investigar lo que los usuarios buscan diariamente, en el intento de hacerlo vos mismo te encontrarás con problemas que solo desembocan en tiempo mal gastado. <br><br>

				Estoy acá para ayudarte a redactar textos empáticos, construidos con palabras claves que posicionan orgánicamente a largo plazo, generan mayor número de visualizaciones y aumentan tus ventas o conversiones.
			  </p>
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
.text{
	text-align: center;
	position: absolute;
	top: 120px;
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
