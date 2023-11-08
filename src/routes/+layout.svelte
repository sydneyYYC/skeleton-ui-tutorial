<script>
	import '../app.postcss';
	import { AppShell, AppBar, Avatar } from '@skeletonlabs/skeleton';
</script>

<!-- App Shell -->
<AppBar>
	<svelte:fragment slot="header">Header</svelte:fragment>
	<svelte:fragment slot="sidebarLeft">Sidebar Left</svelte:fragment>
	<!-- (sidebarRight) -->
	<svelte:fragment slot="pageHeader">Page Header</svelte:fragment>
	<!-- Router Slot -->
	<slot />
	<!-- ---- / ---- -->
	<!-- (pageFooter) -->
	<svelte:fragment slot="footer">&copy;Sydney</svelte:fragment>
</AppBar>
<AppShell>
	<svelte:fragment slot="lead">
		<strong class="text-xl uppercase">Skeleton</strong>
		<p class="mx-4">Hello</p>
	</svelte:fragment>
	<svelte:fragment slot="trail">
		<a
		class="btn btn-sm variant-ghost-surface"
			href="https://discord.gg/EXqV7W8MtY"
			target="_blank"
			rel="noreferrer"
			>
			Discord
		</a>
		<a
		class="btn btn-sm variant-ghost-surface"
		href="https://twitter.com/SkeletonUI"
		target="_blank"
		rel="noreferrer"
		>
		Twitter
	</a>
	<a
	class="btn btn-sm variant-ghost-surface"
	href="https://github.com/skeletonlabs/skeleton"
	target="_blank"
	rel="noreferrer"
	>
	GitHub
</a>
</svelte:fragment>
</AppShell>
<!-- App Bar -->

