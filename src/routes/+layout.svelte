<script>
	import '../app.css';
	import githubLogo from '$lib/images/github-mark.png';
	import gmailLogo from '$lib/images/gmail-logo.png';
</script>

<!--the left navigation bar -->
<div class="flex h-screen">
	<div class="nav-container px-7 py-6 w-72 border-r-2">
		<a href="/">
			<h2 class="text-3xl">Hoonsung Lee</h2>x
			<h3 class="text-xl mb-12">Developer website</h3>
		</a>
		<nav>
			<ul class="text-3xl mb-12">
				<li>
					<a class="group relative inline-block" href="Resume"
						>Resume<span
							class="absolute left-0 right-0 bottom-0 h-0.5 bg-black scale-x-0 group-hover:scale-x-100 transition-transform duration-100 origin-left"
						></span>
					</a>
				</li>
				<li>
					<a class="group relative inline-block" href="Blog"
						>Blog<span
							class="absolute left-0 right-0 bottom-0 h-0.5 bg-black scale-x-0 group-hover:scale-x-100 transition-transform duration-100 origin-left"
						></span>
					</a>
				</li>
				<li>
					<a class="group relative inline-block" href="Projects"
						>Projects<span
							class="absolute left-0 right-0 bottom-0 h-0.5 bg-black scale-x-0 group-hover:scale-x-100 transition-transform duration-100 origin-left"
						></span>
					</a>
				</li>
			</ul>
			<p>Contacts:</p>
			<ul>
				<li>
					<div class="group relative inline-block ml-2">
						<a
							class=" flex items-center text-2xl"
							href="https://github.com/hoonsunglee"
						>
							Github
							<img
								class="w-6 ml-1"
								src={githubLogo}
								alt="A Github Logo"
								draggable="false"
							/>
						</a>
						<span
							class="absolute left-0 right-0 bottom-0 h-0.5 bg-black scale-x-0 group-hover:scale-x-100 transition-transform duration-100 origin-left"
						></span>
					</div>
				</li>
				<li>
					<div class="group relative inline-block ml-2">
						<a
							class=" flex items-center text-2xl"
							href="mailto:hoonsunglee5@gmail.com"
						>
							Email
							<img
								class="w-10"
								src={gmailLogo}
								alt="A Gmail Logo"
								draggable="false"
							/>
						</a>
						<span
							class="absolute left-0 right-0 bottom-0 h-0.5 bg-black scale-x-0 group-hover:scale-x-100 transition-transform duration-100 origin-left"
						></span>
					</div>
				</li>
			</ul>
		</nav>
	</div>
	<div class="flex-1 py-6 px-32">
		<slot />
	</div>
</div>
