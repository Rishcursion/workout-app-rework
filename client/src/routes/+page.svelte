<script>
	import {
		Dumbbell,
		LogInIcon,
		UserPen,
		ArrowRight,
		CalendarIcon,
		TrendingUpIcon,
		LibraryIcon,
		ChartBarBig
	} from 'lucide-svelte';
	import HomeCard from '$lib/home_card.svelte';
</script>

<nav class="container mx-auto px-6 py-2">
	<div class="ml-20 mt-5 flex items-center justify-between">
		<!-- Website Logo/ Nav Bar Left Side -->
		<div class="flex items-center space-x-2 py-5">
			<Dumbbell size={48} class="mx-2 my-2 text-white" />
			<span class="text-4xl font-bold text-white">FitTrack</span>
		</div>
		<!-- Nav Bar Right Side -->
		<div class="m-2 mr-40 mt-5 flex space-x-6">
			<!-- Login Button -->
			<button
				class="mx-4 flex items-center justify-center rounded-full pl-2 pr-4 text-xl font-bold text-white transition delay-100 ease-in hover:bg-white hover:bg-opacity-40 hover:text-indigo-500 hover:backdrop-blur-sm active:bg-opacity-80"
			>
				<LogInIcon class="mr-2" />
				Login
			</button>
			<!-- Register Button -->
			<button
				class="mx-2 flex items-center justify-center rounded-3xl bg-white p-2 px-4 text-xl font-bold text-purple-500 transition delay-100 ease-in hover:bg-indigo-500 hover:text-white active:bg-black"
			>
				<UserPen class="mr-2" />
				Register
			</button>
		</div>
	</div>
</nav>
<!-- Hero -->
<div class="container mx-auto px-6 py-20">
	<div class="text-center">
		<h1 class="mb-7 text-5xl font-bold text-white md:text-6xl">
			Digitize Your Fitness <br /> Journey
		</h1>
		<p class="mx-auto mb-10 max-w-2xl text-xl text-white text-opacity-90">
			Augment your workouts with routine tracking, personalized recommendations and more.
		</p>
		<button
			class="mb-10 inline-flex items-center rounded-full bg-indigo-500 p-4 text-xl font-semibold text-white shadow-md transition ease-in hover:bg-purple-700 hover:bg-opacity-80 active:bg-purple-900 active:bg-opacity-100 active:text-lg"
		>
			Get Started For Free
			<ArrowRight className="h-5 w-5 my-2 ml-2" />
		</button>
	</div>
</div>

<!-- Card Section -->
<div class="container mx-auto w-3/5 px-6 py-20">
	<div class="grid grid-cols-2 gap-8">
		<HomeCard
			title="Progress Tracking"
			icon={ChartBarBig}
			body="Monitor your progress with detailed analytics and
			charts"
		/>
		<HomeCard
			title="Workout Planning"
			icon={CalendarIcon}
			body="Create and customize your workout routines with our intuitive planner."
		/>
		<HomeCard
			title="Goal Setting"
			icon={TrendingUpIcon}
			body="See how far you have come or set your future goals with our goal planner."
		/>
		<HomeCard
			title="Exercise Library"
			icon={LibraryIcon}
			body="Don't know where to start or want to upgrade your routine? Go through our catalogue of excercises with detailed guides."
		/>
	</div>
</div>
