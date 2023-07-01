<script lang="ts">
	import Icon from "./Icon.svelte";
</script>

<div class="px-6 py-4 m-2 bg-gray-800 rounded-lg">
	<button
		class="flex items-center justify-start mb-3 text-lg text-white hover:text-slate-100"
	>
		<Icon icon="ic:round-home" class="mr-2 text-2xl" /> Home
	</button>

	<button
		class="flex items-center justify-start mb-3 text-lg text-slate-300 hover:text-slate-100"
	>
		<Icon icon="ic:baseline-explore" class="mr-2 text-2xl" /> Explore
	</button>

	<button
		class="flex items-center justify-start mb-3 text-lg text-slate-300 hover:text-slate-100"
	>
		<Icon icon="ic:baseline-library-music" class="mr-2 text-2xl" /> Library
	</button>

	<button
		class="flex items-center justify-start text-lg text-slate-300 hover:text-slate-100"
	>
		<Icon icon="ic:baseline-history" class="mr-2 text-2xl" /> History
	</button>
</div>

<div class="px-6 py-4 m-2 mt-4 bg-gray-800 rounded-lg">
	<h2 class="flex items-center mb-2 text-lg font-semibold text-slate-300">
		<Icon icon="ic:baseline-playlist-play" class="mr-2 text-4xl" /> Playlists
	</h2>

	<button
		class="flex items-center justify-start w-full py-1 mb-1 text-sm rounded text-slate-300 hover:bg-slate-700"
	>
		Playlist 1
	</button>
	<button
		class="flex items-center justify-start w-full py-1 mb-1 text-sm rounded text-slate-300 hover:bg-slate-700"
	>
		Bored apes
	</button>
	<button
		class="flex items-center justify-start w-full py-1 mb-1 text-sm rounded text-slate-300 hover:bg-slate-700"
	>
		Playlist 5
	</button>
	<button
		class="flex items-center justify-start w-full py-1 mb-1 text-sm rounded text-slate-300 hover:bg-slate-700"
	>
		NEW PLAYLIST
	</button>
	<button
		class="flex items-center justify-start w-full py-1 mb-1 text-sm rounded text-slate-300 hover:bg-slate-700"
	>
		Good songs
	</button>
</div>
