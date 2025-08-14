<script>
	export let data;
	import validrss from "/assets/buttons/validrss.png";
	import validatom from "/assets/buttons/validatom.png";
</script>

<style>
img {
    width: 88px;
    height: 31px;
}
</style>

## My super cool blog!

if i ever decide to, my blogs are written here, here they are: (now posting more frequently!)

<ul>
{#each data.posts as post}
<li><a href="{post.path}">{post.meta.title}</a> | {post.meta.date}</li>
{/each}
</ul>

## Get notified

if you wish to magically know when i release a new thought into this river of posts, add my atom or RSS feed to your preferred client!

- [<i class="fa-solid fa-atom"></i> atom feed](/blog/atom.xml)
- [<i class="fa-solid fa-rss"></i> legacy RSS feed](/blog/rss.xml)

[![valid atom]({validatom})](https://validator.w3.org/feed/check.cgi?url=https%3A//t480.dev/blog/atom.xml)
[![valid rss]({validrss})](https://validator.w3.org/feed/check.cgi?url=https%3A//t480.dev/blog/rss.xml)
