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
</style>

<Nav {segment}/>

<main class=" bg-gray-200"	>
	<div class="grid gap-4 grid-cols-3">
		<div class="col-span-2  m-10 bg-white"><slot ></slot></div>	
		<div class="col-span-1   m-10"><Contact contact_info={DATA.CONTACT_DATA}/></div>
	  </div>

	  <Footer/>
</main>

