<script lang="ts">
	import Icon from "./Icon.svelte";
</script>

<div class="flex items-center px-6 py-4 m-2 bg-gray-800 rounded-lg select-none">
	<h1
		class="text-2xl font-semibold text-gray-400 cursor-pointer active:scale-95"
	>
		Musicify
	</h1>

	<div class="flex items-center gap-2 mx-4">
		<button
			class="inline-flex items-center justify-center w-8 h-8 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
		>
			<Icon icon="icon-park-outline:left" />
		</button>

		<button
			class="inline-flex items-center justify-center w-8 h-8 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
		>
			<Icon icon="icon-park-outline:right" />
		</button>
	</div>

	<input
		type="text"
		class="flex-1 px-4 py-2 text-white border-none rounded-lg outline-none placeholder:text-slate-400 focus:ring-2 bg-slate-700"
		placeholder="Search"
	/>

	<div class="flex items-center gap-2 ml-4">
		<button
			class="inline-flex items-center justify-center w-8 h-8 p-1 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
		>
			<Icon icon="ic:baseline-notifications" />
		</button>

		<button
			class="inline-flex items-center justify-center w-8 h-8 p-1 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
		>
			<Icon icon="ic:sharp-settings" />
		</button>

		<button
			class="inline-flex items-center justify-center w-8 h-8 p-1 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
		>
			<Icon icon="clarity:logout-line" />
		</button>
	</div>
</div>
