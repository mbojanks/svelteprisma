<script lang="ts">
    import { i } from '@inlang/sdk-js';
	import '@picocss/pico'
</script>

<div class="container">
	<hgroup>
		<h1>
			<a href="/"> SvelteKit & Prisma 🔥</a>
		</h1>

		<h2>{i("intro")}</h2>
	</hgroup>
	<slot />
</div>