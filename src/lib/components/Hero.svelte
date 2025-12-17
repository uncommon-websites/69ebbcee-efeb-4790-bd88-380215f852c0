<script>
	const stats = [
		{ value: '7-8 Figure', label: 'Amazon Brands' },
		{ value: '$600B', label: 'Market Opportunity' },
		{ value: 'Profit-First', label: 'Strategy' }
	];
</script>

<section class="relative overflow-hidden border-b border-gray-200 bg-white pt-20 pb-16">
	<!-- Geometric Decoration Top Right -->
	<div class="absolute top-0 right-0 h-64 w-64 opacity-10 pointer-events-none">
		<svg viewBox="0 0 100 100" class="h-full w-full stroke-gray-400" fill="none">
			<path d="M0 0 L100 100 M50 0 L100 50 M0 50 L50 100" stroke-width="0.5" />
			<rect x="50" y="0" width="50" height="50" stroke-width="0.5" />
		</svg>
	</div>

	<!-- Geometric Decoration Top Left -->
	<div class="absolute top-0 left-0 h-64 w-64 opacity-10 pointer-events-none">
		<svg viewBox="0 0 100 100" class="h-full w-full stroke-gray-400" fill="none">
			<circle cx="50" cy="50" r="40" stroke-width="0.5" />
			<circle cx="50" cy="50" r="25" stroke-width="0.5" />
		</svg>
	</div>

	<div class="mx-auto max-w-[1400px] px-6">
		<div class="max-w-4xl mx-auto text-center">
			<!-- Badge -->
			<a href="#" class="mb-8 inline-flex items-center gap-2 rounded-full border border-primary-200 bg-primary-50 px-3 py-1 text-[10px] font-bold tracking-widest text-primary-700 hover:bg-primary-100 uppercase">
				<span class="text-primary-500">Owner-Led</span>
				Built & Exited My Own Amazon Brand &rsaquo;
			</a>

			<!-- Headline -->
			<h1 class="mb-6 text-7xl font-medium tracking-tight text-gray-900">
				Transform Your Amazon Brand Into a Profit Engine
			</h1>

			<!-- Subhead -->
			<p class="mb-10 mx-auto max-w-2xl text-lg leading-relaxed text-gray-600">
				Stop wasting money on inconsistent agency results. Get <strong class="font-semibold text-gray-900">owner-led strategy and hands-on execution</strong> from someone who's built, scaled, and exited their own 7-figure Amazon brand.
			</p>

			<!-- Buttons -->
			<div class="mb-24 flex items-center justify-center gap-4">
				<a href="#" class="bg-gray-900 px-6 py-3 text-[11px] font-bold tracking-widest text-white transition-colors hover:bg-gray-800 uppercase">
					Book Strategy Call
				</a>
				<a href="#" class="border border-gray-200 bg-white px-6 py-3 text-[11px] font-bold tracking-widest text-gray-900 transition-colors hover:bg-gray-50 uppercase">
					View Case Studies
				</a>
			</div>
		</div>

		<!-- Stats -->
		<div class="flex flex-wrap items-center justify-center gap-12 border-t border-primary-100 pt-8">
			{#each stats as stat}
				<div class="text-center">
					<div class="text-3xl font-bold text-primary-700">{stat.value}</div>
					<div class="text-xs font-semibold tracking-widest text-gray-500 uppercase">{stat.label}</div>
				</div>
			{/each}
		</div>
	</div>
</section>