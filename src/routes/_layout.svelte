<script>
	import Nav from '../components/Nav.svelte';
	import Contact from '../components/Contact.svelte';
	import Footer from '../components/Footer.svelte';
	import DATA from '../Data/data.js';
	export let segment;
</script>

<style global>
    @tailwind base;
    @tailwind components;
    @tailwind utilities;

	.lg\:mx-width-30 {
		min-width: min(100vw, 350px);
		max-width: 30%;
	}

	:global(#sapper) {
		position: relative;
		padding-top: 55px;
		width: 100%;
		min-height: 100vh;
		display: flex;
		flex-direction: column;
	}

	main {
		flex-grow: 1;
		min-height: 100%;
	}

	@media screen and (max-width: 1024px) {
		.lg\:mx-width-30 {
			margin-left: 0;
			max-width: 100%;
		}
	}

	.ac {
		min-height: 100%;
		max-width: 100%;
		width: calc(100% - 5em);
	}
</style>

<Nav {segment}/>
<main class="flex flex-col bg-gray-200 min-h-full">
	<div class="flex lg:flex-row flex-col min-h-full max-w-full w-full">
		<div class="m-10 bg-white ac">
			<slot></slot>
		</div>	
		<div class="col-span-1 m-10 lg:m-5 lg:mx-width-30 h-full ">
			<Contact contact_info={DATA.CONTACT_DATA}/>
		</div>
	</div>
</main>
<Footer/>
