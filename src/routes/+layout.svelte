<script lang="ts">
	import '../app.css';
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<title>Sasan Jaghori</title>
</svelte:head>

<div class="min-h-screen flex flex-col justify-between pt-0 md:pt-8 p-8 bg-white text-gray-900">
	<main class="max-w-[60ch] mx-auto w-full space-y-6">
		<slot />
	</main>
	<Footer />
	<!-- <Analytics /> -->
</div>
