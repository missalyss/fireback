<script>
	import './layout.css';
	  import '../app.css'

	import favicon from '#lib/assets/favicon.svg';

	/** @type {{children: import('svelte').Snippet}} */
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<nav class="text-white bg-blues p-10">

	<a class="px-10 button text-only fire-20 text-xl" href="/">Home</a>
	<a class="px-10 button text-only fire-20 text-xl" href="/about">About</a>
	<a class="px-10 button text-only fire-20 text-xl" href="/contact">Contact</a>
</nav>
<main class=" bg-white rounded-md m-10 p-10">
	{@render children()}
</main>
<footer class="text-white bg-blues p-10">

	<a class="px-10 button text-only fire-20 text-xl" href="/">Footer Link</a>
	<a class="px-10 button text-only fire-20 text-xl" href="/about">About</a>
	<a class="px-10 button text-only fire-20 text-xl" href="/contact">Contact</a>
	<p class="px-10">FireBack 2026</p>
</footer>
