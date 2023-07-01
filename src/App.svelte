<script lang="ts">
	import Header from "./Header.svelte";
	import Player from "./Player.svelte";
	import Sidebar from "./Sidebar.svelte";
</script>

<Header />

<div class="grid grid-cols-12">
	<div class="col-span-3">
		<Sidebar />
	</div>

	<div class="col-span-9 p-4 m-2 rounded-lg max-h-[calc(100vh-220px)] overflow-auto bg-slate-800">
		<div class="grid grid-cols-4 gap-4">
			<div
				class="col-span-1 text-center bg-[#1DB954] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/popular/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Popular</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#FF6B6B] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/trending/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Trending</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#3490DC] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/new-releases/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">New Releases</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#F59E0B] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/featured/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Featured</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#9333EA] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/best-sellers/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Best Sellers</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#10B981] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/top-hits/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Top Hits</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#6366F1] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/editors-picks/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Editor's Picks</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#EC4899] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/classics/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Classics</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#14B8A6] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/party-mix/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Party Mix</h1>
			</div>

			<div
				class="col-span-1 text-center bg-[#FCD34D] rounded-lg hover:-translate-y-1 cursor-pointer transition-all p-4"
			>
				<img
					src="https://picsum.photos/seed/mellow-vibes/200/200"
					alt="album"
					class="w-24 m-auto mb-4 rounded-lg shadow-lg rotate-3"
				/>
				<h1 class="text-2xl font-semibold text-white">Mellow Vibes</h1>
			</div>
		</div>
	</div>
</div>

<Player />
