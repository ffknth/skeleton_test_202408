<script lang="ts">
	import '../app.postcss';
	import {AppShell} from '@skeletonlabs/skeleton';
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
	<svelte:fragment slot="sidebarLeft">
		<!-- Insert the list: -->
		<div class="container" style="position: fixed;  box-sizing: border-box; width: 200px; height: 100%;" >
			<nav class="list-nav">
				<ul>
					<li><a href="/">Home</a></li>
					<li><a href="/about">About</a></li>
					<li><a href="/news">News</a></li>
					<li><a href="/news">Documents</a></li>
					<li><a href="/news">Examples</a></li>
					<li><a href="/about">Contact</a></li>
				</ul>
			</nav>
		</div>
		<!-- --- -->
	</svelte:fragment>
</AppShell>
<slot />
