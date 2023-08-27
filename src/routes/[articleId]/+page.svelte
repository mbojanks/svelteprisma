<script lang="ts">
	import type { PageData } from './$types'
	import { i } from '@inlang/sdk-js';
	export let data: PageData
	$: ({ article } = data)
</script>
<form action="?/updateArticle" method="POST">
	<h3>{i("editing")}: {article.title}</h3>
	<label for="title"> {i("title")} </label>
	<input type="text" id="title" name="title" value={article.title} />
	<label for="content"> {i("content")}</label>
	<textarea id="content" name="content" rows={5} value={article.content} />
	<button type="submit">{i("update")}</button>
    <a href="/" role="button" class="outline constrast" style="width: 100%;"
					>{i("backtoarticles")}</a>
</form>