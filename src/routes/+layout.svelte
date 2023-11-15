<script>
	import { Button } from 'flowbite-svelte';
	import '../app.postcss';
	import '../app.scss';
	import { AppShell, AppBar, AppRail } from '@skeletonlabs/skeleton';
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
<Button><a href="login">Login</a></Button>
<AppBar>Bar</AppBar>
<AppRail>Rail</AppRail>
</AppShell>
<slot />
