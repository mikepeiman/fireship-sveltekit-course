<script>
	import {
		Button,
		Alert,
		Card,
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		Toast
	} from 'flowbite-svelte';
	import { FireOutline } from 'flowbite-svelte-icons';
	import Icon from '@iconify/svelte';
  let hidden = true
</script>

<Button color="primary">Primary</Button>
<Alert color="primary">Primary</Alert>
<Card href="/cards" color="primary" class="bg-white">
	<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-red-800">
		Noteworthy technology acquisitions 2021
	</h5>
	<p class="font-normal text-gray-700 dark:text-gray-700 leading-tight">
		Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological
		order.
	</p>
</Card>
<Navbar let:hidden let:toggle color="primary">
	<NavBrand href="/">
		<Icon icon="mdi-light:home" class="text-4xl text-cyan-500" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-red-800"
			>Flowbite</span
		>
	</NavBrand>
	<NavHamburger on:click={toggle} />
	<NavUl {hidden}>
		<NavLi href="/" active={true}>Home</NavLi>
		<NavLi href="/about">About</NavLi>
		<NavLi href="/services">Services</NavLi>
		<NavLi href="/pricing">Pricing</NavLi>
		<NavLi href="/contact">Contact</NavLi>
	</NavUl>
</Navbar>
<Toast color="primary">
	<svelte:fragment slot="icon">
		<!-- <FireOutline class="w-6 h-6" /> -->
    <Icon icon="mdi-light:home" class="text-4xl text-cyan-500" />
	</svelte:fragment>
	Dismissable user notification.
</Toast>
