<script>
	import Hero from '$lib/components/Hero.svelte';
	import FeaturedApps from '$lib/components/FeaturedApps.svelte';
	import ComingSoon from '$lib/components/ComingSoon.svelte';
	import Manifesto from '$lib/components/Manifesto.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
	<title>Bretzel — Self-hosted apps, baked in Europe</title>
	<meta name="description" content="Bretzel is a suite of open source, self-hosted web apps. Privacy-first, EU-made, no cloud required." />
</svelte:head>

<main class="min-h-screen">
	<Hero />
	<FeaturedApps />
	<ComingSoon />
	<Manifesto />
</main>
<Footer />
