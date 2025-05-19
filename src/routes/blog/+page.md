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

## My blog, or "fountain"

if i ever decide to, my blogs or "scrolls" are written here, here they are:

<ul>
{#each data.posts as post}
<li><a href="{post.path}">{post.meta.title}</a> | {post.meta.date}</li>
{/each}
</ul>

## Get notified

I have an Atom feed (don't use, under maintenance) and an RSS feed if you wish to be notified whenever I update my "scroll"!

- [<i class="fa-solid fa-atom"></i> atom feed](/blog/rss.xml)
- [<i class="fa-solid fa-rss"></i> legacy rss feed](/blog/rss.xml)

[![valid atom]({validatom})](https://validator.w3.org/feed/check.cgi?url=https%3A//t480.dev/blog/atom.xml)
[![valid rss]({validrss})](https://validator.w3.org/feed/check.cgi?url=https%3A//t480.dev/blog/rss.xml)
