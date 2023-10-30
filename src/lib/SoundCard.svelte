<script lang="ts">
	export let sound: string;
	let soundPath = `/${sound}.mp3`;
</script>

<div class="card">
	<h3>{sound}</h3>
	<audio controls loop>
		<source src={soundPath} type="audio/mp3" />
		Your browser does not support the audio element.
	</audio>
</div>

<style>
	.card {
		border: 1px solid #ddd;
		border-radius: 8px;
		overflow: hidden;
		background-color: white;
		padding: 20px;
		box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
	}

	audio {
		width: 100%;
		display: block;
		outline: none;
	}

	@media (max-width: 768px) {
		.card {
			width: 90%;
			margin: 0 auto;
		}
	}
</style>
