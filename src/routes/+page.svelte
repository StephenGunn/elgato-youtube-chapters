<script lang="ts">
	import '$lib/styles/reset.css';
	import '$lib/styles/app.css';
	import Converter from './Converter.svelte';
	import Header from './Header.svelte';
	import Hero from './Hero.svelte';
	import Footer from './Footer.svelte';
	import HowToUse from './HowToUse.svelte';
</script>

<main>
	<Header />
	<Hero />
	<Converter />
	<HowToUse />
	<Footer />
</main>
