<script>
	export let segment;
  </script>


<nav class="flex items-center justify-between flex-wrap bg-red-700 p-3">
	<div class=" text-white mr-1 flex flex-wrap ">
	  <div class="font-semibold text-lg tracking-tight w-3/5">Emilie Bout</div>
	  <div class="  tracking-tight text-xs">Ph.D Student in Computer Science</div>
	</div>
	<div class="block lg:hidden">
	  <button class="flex items-center px-3 py-2 border rounded text-white border-teal-400 hover:text-white hover:border-white">
		<svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
	  </button>
	</div>
	<div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
	  <div class="text-sm lg:flex-grow">
		<a href="about" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white mr-4">
		  About
		</a>
		<a href="cv" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white mr-4">
		  Curriculum Vitae
		</a>
		<a href="publication" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white mr-4" class:selected={segment === undefined}>
		  Publications
		</a>
		<a href="teaching" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white mr-4">
		  Teaching
		</a>
		  </div>
	  <div>
		<a href="https://www.inria.fr/fr"><img src='logo.png' class=" h-8 inline-block  mt-4 lg:mt-0"></a>
	  </div>
	</div>
  </nav>






