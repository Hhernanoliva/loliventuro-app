<script>
	import Footer from '$lib/Footer/index.svelte';
	import Header from '$lib/Header/index.svelte';
</script>


<div class="app">
	<Header />
		<slot />
	<Footer />
</div>

<style>
.app{
	background: #5f4b8b;
	width:  100vw;
	height: 100vh;
	display: flex;
	flex-direction: column;
	color: white;
}
@media (max-width: 767.98px) {
	.app{
	background-position: 65%;
}
.layer{
	height: 100vh;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

}
:global(body) {
		overflow: hidden;
		margin: 0;
	}

</style>
