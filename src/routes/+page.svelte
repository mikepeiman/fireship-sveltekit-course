<script>
	import FlowbiteExample1 from '../components/FlowbiteExample1.svelte';
	import { Button } from 'flowbite-svelte';
</script>

<div class="w-full">
	<div class="p-24">
		<div class="bg-blue-900 p-24 rounded-[2rem]">
			<div class="flex flex-col flex-1 justify-center items-center">
				<h1 class="text-cyan-400 text-4xl">Welcome to SvelteKit</h1>
				<Button><a href="login">Login</a></Button>
				<FlowbiteExample1 />
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	/* your styles go here */
</style>
