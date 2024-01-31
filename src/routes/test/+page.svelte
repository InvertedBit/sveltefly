<script lang="ts">
	import { json } from "@sveltejs/kit";
import type { PageData } from "./$types";

export let data: PageData
</script>

<svelte:head>
	<title>API Test</title>
	<meta name="description" content="Firefly API test" />
</svelte:head>

<section>
	<h1>
		API Test
	</h1>
    

    <pre>
        {JSON.stringify(data, null, 2)}
    </pre>
    

    <button>Call API now!</button>


</section>