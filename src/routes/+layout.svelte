<script>
	import Header from '$lib/Header.svelte';
	import SideBar from '$lib/SideBar.svelte';
</script>

<Header />
<div class="app">
	<slot />
	<SideBar />
</div>

<style>
	div {
		display: flex;
	}
</style>
