<script>
	/**
	 * @type string
	 */
	export let title;
	/**
	 * @type string
	 */
	export let date;
	/**
	 * @type string
	 */
	export let modified;
</script>

<svelte:head>
	<title>{title} | charlie's blog</title>
	<meta name="description" content="charlie's comfy blog" />
	<meta property="og:title" content="{title} | charlie's blog" />
	<meta property="og:description" content="charlie's comfy blog" />
</svelte:head>

<p><a href="https://t480.dev/blog"><i class="fa-solid fa-arrow-left"></i> back to my blog</a></p>

<h2>{title}</h2>
<p>publish date: {date}</p>
{#if modified}
	<p>modified date: {modified}</p>
{/if}
<p>author: charlie (a53x@shitposting.expert)</p>
<hr />
<slot />
