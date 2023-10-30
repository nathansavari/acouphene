<script lang="ts">
	import SoundCard from '$lib/SoundCard.svelte';

	let sounds = ['Abysse', 'Abysse2']; // Add your sound names here
</script>

<div class="card--section">
	{#each sounds as sound (sound)}
		<SoundCard {sound} />
	{/each}
</div>

<style>
	div {
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		gap: 20px;
		width: 100vw;
		max-width: 90vw;
		align-items: center;
		padding: 20px;
	}

	@media (max-width: 768px) {
		div {
			grid-template-columns: 2fr;
		}
	}

	@media (max-width: 480px) {
		div {
			grid-template-columns: 1fr;
		}
	}
</style>
