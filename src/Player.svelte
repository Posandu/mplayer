<script lang="ts">
	import Icon from "./Icon.svelte";

	let progress = 0;

	setInterval(() => {
		progress += 1;
	}, 1000);

	$: if (progress >= 180) {
		progress = 0;
	}
</script>

<div
	class="fixed bottom-0 z-50 flex w-full px-6 py-4 m-2 rounded-lg bg-slate-900"
>
	<div class="flex items-center">
		<img
			src="https://picsum.photos/50/50"
			class="w-12 h-12 rounded-full"
			alt="profile"
		/>

		<div class="flex flex-col ml-4">
			<h3
				class="text-lg font-semibold text-white cursor-pointer hover:underline"
			>
				Feel Good Inc.
			</h3>
			<p class="text-sm cursor-pointer text-slate-400 hover:underline">
				Gorillaz
			</p>
		</div>
	</div>

	<div class="flex flex-col items-center flex-1">
		<div class="flex items-center">
			<button
				class="inline-flex items-center justify-center w-8 h-8 p-1 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
			>
				<Icon icon="ic:baseline-skip-previous" />
			</button>

			<button
				class="inline-flex items-center justify-center w-10 h-10 p-1 mx-2 text-3xl text-white transition-all bg-blue-600 rounded-full active:scale-95 hover:bg-opacity-80"
			>
				<Icon icon="ic:baseline-pause" />
			</button>

			<button
				class="inline-flex items-center justify-center w-8 h-8 p-1 mr-2 text-2xl text-white bg-white rounded-full active:scale-95 hover:bg-opacity-25 bg-opacity-10"
			>
				<Icon icon="ic:baseline-skip-next" />
			</button>

			<button
				class="inline-flex items-center justify-center w-8 h-8 p-1 text-2xl text-white rounded-full bg-slate-500 active:scale-95 hover:bg-opacity-25 bg-opacity-10"
			>
				<Icon icon="ic:baseline-repeat" />
			</button>

			<button
				class="inline-flex items-center justify-center w-8 h-8 p-1 ml-2 text-2xl text-white rounded-full bg-slate-500 active:scale-95 hover:bg-opacity-25 bg-opacity-10"
			>
				<Icon icon="ic:baseline-shuffle" />
			</button>
		</div>

		<div class="flex mt-3">
			<span class="mx-2 text-sm text-slate-400">
				{(progress / 60).toFixed(0)}:{(progress % 60)
					.toFixed(0)
					.padStart(2, "0")}
			</span>

			<input
				type="range"
				class="w-full min-w-[400px] h-1 mt-2 rounded-full bg-slate-500"
				bind:value={progress}
				min="0"
				max="180"
			/>
			<span class="mx-2 text-sm text-slate-400"> 4:00 </span>
		</div>
	</div>
</div>
