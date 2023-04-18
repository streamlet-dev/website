<!-- Navbar goes here -->
<nav class="bg-darkblue shadow-lg">
	<div class="max-w-6xl mx-auto px-4">
		<div class="flex justify-between">
			<div class="flex space-x-7">
				<div>
					<!-- Website Logo -->
					<a href="/" class="flex items-center py-4 px-2">
						<img src="/img/streamlets.png" alt="Logo" class="h-8 w-8 mr-2" />
						<span class="font-semibold text-slate-300 text-lg">streamlet.dev</span>
					</a>
				</div>

				<!-- Primary Navbar items -->
				<div class="hidden md:flex items-center space-x-1">
					<a
						href="product"
						class="py-4 px-2 text-slate-300 font-semibold hover:text-slate-500 transition duration-300"
						>Product</a
					>
					<a
						href="company"
						class="py-4 px-2 text-slate-300 font-semibold hover:text-slate-500 transition duration-300"
						>Company</a
					>
				</div>
			</div>
			<!-- Secondary Navbar items -->
			<div class="hidden md:flex items-center space-x-3 ">
				<a
					href="contact"
					class="py-2 px-2 font-medium text-white bg-slate-500 rounded hover:bg-slate-400 transition duration-300"
					>Sign Up</a
				>
			</div>

			<!-- Mobile menu button -->
			<div class="md:hidden flex items-center">
				<button class="outline-none mobile-menu-button">
					<svg
						class=" w-6 h-6 text-slate-300 hover:text-slate-500 "
						x-show="!showMenu"
						fill="none"
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						viewBox="0 0 24 24"
						stroke="currentColor"
					>
						<path d="M4 6h16M4 12h16M4 18h16" />
					</svg>
				</button>
			</div>
		</div>
	</div>

	<!-- mobile menu -->
	<div class="hidden mobile-menu">
		<ul class="">
			<li class="active">
				<a href="index.html" class="block text-sm px-2 py-4 text-white bg-slate-500 font-semibold"
					>Home</a
				>
			</li>
			<li>
				<a
					href="#services"
					class="block text-sm px-2 py-4 text-slate-200 hover:bg-slate-500 transition duration-300"
					>Services</a
				>
			</li>
			<li>
				<a
					href="#about"
					class="block text-sm px-2 py-4 text-slate-200  hover:bg-slate-500 transition duration-300"
					>About</a
				>
			</li>
			<li>
				<a
					href="#contact"
					class="block text-sm px-2 py-4 text-slate-200 hover:bg-slate-500 transition duration-300"
					>Contact Us</a
				>
			</li>
		</ul>
	</div>
	<script>
		const btn = document.querySelector('button.mobile-menu-button');
		const menu = document.querySelector('.mobile-menu');

		btn.addEventListener('click', () => {
			menu.classList.toggle('hidden');
		});
	</script>
</nav>
