<script lang="ts">
	const name = 'Sasan Jaghori';
	const shortName = 'sjaghori';

	// Split name into individual letters for rendering
	const nameArray = name.split('');
	const shortNameArray = shortName.split('');
</script>

<h1 class="font-medium pt-12 transition-element">
	<span class="sr-only">Sasan Jaghori</span>
	<span aria-hidden="true" class="block overflow-hidden group relative">
		<!-- First animated block -->
		<span
			class="inline-block transition-all duration-300 ease-in-out group-hover:-translate-y-full"
		>
			{#each nameArray as letter, index}
				<span class="inline-block" style="transition-delay: {index * 25}ms">
					{letter === ' ' ? '\u00A0' : letter}
				</span>
			{/each}
		</span>

		<!-- Second animated block -->
		<span
			class="inline-block absolute left-0 top-0 transition-all duration-300 ease-in-out translate-y-full group-hover:translate-y-0"
		>
			{#each shortNameArray as letter, index}
				<span class="inline-block" style="transition-delay: {index * 25}ms">
					{letter}
				</span>
			{/each}
		</span>
	</span>
</h1>
