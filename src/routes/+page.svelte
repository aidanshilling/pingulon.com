<script lang="ts">
	import type { PageProps } from "./$types";
	import { marked } from "marked";

	let { data }: PageProps = $props();
</script>

<div>{@html marked.parse(data.story.body)}</div>
