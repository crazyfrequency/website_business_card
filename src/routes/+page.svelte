<script>
	import Header from "$lib/components/Header.svelte";
    import Line from "$lib/components/Line.svelte";
    import Description from "$lib/components/Description.svelte";
    import Possibilities from "$lib/components/Possibilities.svelte";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div>
	<Header />
	<Line />
	<Description />
	<Line />
	<Possibilities />
</div>
