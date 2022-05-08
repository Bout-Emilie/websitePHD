<script>
	export let segment;

	let isSubMenuActive = false;

	const handle_show_sub_menu = () => isSubMenuActive = !isSubMenuActive;
	const hide_menu = () => isSubMenuActive = false;
  </script>

<!-- TODO: Adding Inria icon in responsive -->
<header class={`flex fixed top-0 w-full items-center ${isSubMenuActive ? 'justify-center' : 'justify-between'} flex-wrap bg-red-700 p-3 z-50`}>
	<div class={`text-white lg:mr-1 flex flex-wrap flex-col ${isSubMenuActive ? 'items-center my-3' : 'items-start'}`}>
	  <div class="font-semibold text-lg tracking-tight w-3/5">Emilie Bout</div>
	  <div class="  tracking-tight text-xs text-center">Ph.D Student in Computer Science</div>
	</div>
	<div class={`lg:hidden ${isSubMenuActive ? 'hidden' : 'block'}`} on:click={handle_show_sub_menu}>
	  <button class="flex items-center px-3 py-2 border rounded text-white border-teal-400 hover:text-white hover:border-white">
		<svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
			<title>Menu</title>
			<path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/>
		</svg>
	  </button>
	</div>
	<div class={`w-full flex-grow lg:flex lg:items-center lg:w-auto ${isSubMenuActive ? 'flex' : 'hidden'} flex-col lg:flex-row items-center `}>
	  <div class="text-sm flex lg:flex-grow flex-col lg:flex-row justify-center items-center my-1 lg:my-0">
		<a href="about" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white lg:mr-4" on:click={hide_menu}>
		  About
		</a>
		<a href="cv" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white lg:mr-4" on:click={hide_menu}>
		  Curriculum Vitae
		</a>
		<a href="publication" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white lg:mr-4" class:selected={segment === undefined} on:click={hide_menu}>
		  Publications
		</a>
		<a href="technical" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white lg:mr-4" class:selected={segment === undefined} on:click={hide_menu}>
			Technical Report
		  </a>
		<a href="teaching" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white lg:mr-4" on:click={hide_menu}>
		  Teaching
		</a>
		<a href="communication" class="block mt-4 lg:inline-block lg:mt-0 text-white hover:text-white lg:mr-4" on:click={hide_menu}>
			Communication
		  </a>
		  </div>
	  <div>
		<a href="https://www.inria.fr/fr" target="_blank" rel="nofollow" class="hidden lg:block">
			<img src='logo.png' alt="logo" class=" h-8 inline-block  mt-4 lg:mt-0">
		</a>
	  </div>
	  <div class="block lg:hidden my-3" on:click={handle_show_sub_menu}>
		<button class="flex items-center px-3 py-2 border rounded text-white border-teal-400 hover:text-white hover:border-white">
			<svg class="fill-current h-3 w-3" viewBox="0 0 329.26933 329"xmlns="http://www.w3.org/2000/svg"><path d="m194.800781 164.769531 128.210938-128.214843c8.34375-8.339844 8.34375-21.824219 0-30.164063-8.339844-8.339844-21.824219-8.339844-30.164063 0l-128.214844 128.214844-128.210937-128.214844c-8.34375-8.339844-21.824219-8.339844-30.164063 0-8.34375 8.339844-8.34375 21.824219 0 30.164063l128.210938 128.214843-128.210938 128.214844c-8.34375 8.339844-8.34375 21.824219 0 30.164063 4.15625 4.160156 9.621094 6.25 15.082032 6.25 5.460937 0 10.921875-2.089844 15.082031-6.25l128.210937-128.214844 128.214844 128.214844c4.160156 4.160156 9.621094 6.25 15.082032 6.25 5.460937 0 10.921874-2.089844 15.082031-6.25 8.34375-8.339844 8.34375-21.824219 0-30.164063zm0 0"/></svg>
		</button>
	  </div>
	</div>
  </header>






