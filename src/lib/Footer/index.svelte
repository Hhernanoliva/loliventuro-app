<script>
	import { page } from '$app/stores';
	import IconAbout from '$lib/components/Iconabout.svelte'
	import IconAsistencia from '$lib/components/Iconasistencia.svelte'

</script>

<footer>
	<nav>
		<ul>
			
			<li class:active={$page.path === '/about'}> <a sveltekit:prefetch href="/about"><IconAbout /> Sobre Mi </a></li>
			<li class:active={$page.path === '/asis'}><a sveltekit:prefetch href="/asis"><IconAsistencia style="margin-bottom: 10px;"/> MORA </a></li>
		</ul>
	</nav>
</footer>

<style>
	footer {
		font-family: 'Lato', sans-serif;
		width: 100%;
		position: absolute;
		bottom: 0;
		display: flex;
		justify-content: center;
		z-index: 5;
		background-color: #ffb3dd7c;
		box-shadow: 0px -1px 5px rgba(0, 0, 0, 0.25);
	}

	nav {
		max-width: 600px ;
		display: flex;
		justify-content: center;
		--background: none;
	}

	ul {
		width: 100%;
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: space-around;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;

	}

	li.active::before {
		--size: 6px;
		content: '';
		width: 100%;
		height: 0;
		position: absolute;
		bottom: 10px;
		left: calc(0% - var(--size));
		border: var(--size) solid transparent;
		border-bottom: var(--size) solid var(--accent-color);
		

	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 2em;
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 10%;
		text-decoration: none;
		transition: color 0.2s linear;
		text-shadow: 1px 1px 1px rgba(66, 20, 60, 0.8);
		color: #fff;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	a:hover {
		color: #5f4b8b;
	}
</style>
