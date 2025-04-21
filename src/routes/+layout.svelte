<script lang="ts">
	import '$styles/main.scss';
	import SiteHeader from '$components/SiteHeader.svelte';
	import SiteFooter from '$components/SiteFooter.svelte';
	let { children } = $props();
</script>

<SiteHeader />
<main id="main" class="container" data-type="wide">
	{@render children()}
</main>
<SiteFooter />

<style lang="scss">
	#main {
		min-height: 100svh;
		padding: 2rem 0;
	}
</style>