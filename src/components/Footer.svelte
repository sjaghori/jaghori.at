<script lang="ts">
	const links = [
		{ name: 'linkedin', url: 'https://www.linkedin.com/in/jaghori' },
		{ name: 'github', url: 'https://github.com/sjaghori' }
	];
</script>

<footer class="mt-12 text-center">
	<div class="flex justify-center space-x-4 tracking-tight">
		{#each links as link (link.name)}
			<a
				href={link.url}
				target="_blank"
				rel="noopener noreferrer"
				class="text-gray-400 hover:text-blue-500 transition-colors duration-200">{link.name}</a
			>
		{/each}
		<a
			href="mailto:jaghori.sasan@outlook.com"
			class="text-gray-400 hover:text-blue-500 transition-colors duration-200">email</a
		>
	</div>
</footer>
