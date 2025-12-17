<script>
	let openIndex = 0;
	const faqs = [
		{
			question: "Who is ALFI for?",
			answer: "ALFI is built for 7-8 figure Amazon brand owners who are tired of inconsistent agency results and want profit-focused growth strategies from someone who's actually built, scaled, and exited their own Amazon brand."
		},
		{
			question: "How is ALFI different from other Amazon agencies?",
			answer: "Unlike agencies that learn on your dime, Naeela brings real owner experience. She's navigated every challenge you're facing and focuses on profit-first strategies, not vanity metrics."
		},
		{
			question: "What services does ALFI offer?",
			answer: "We offer comprehensive Amazon optimization including PPC management, listing optimization, inventory planning, operations strategy, and hands-on execution to drive profitable growth."
		},
		{
			question: "How quickly can I expect to see results?",
			answer: "Most clients see measurable improvements in key metrics within 60-90 days. We focus on sustainable, profit-driven growth rather than quick wins that don't last."
		},
		{
			question: "Do you work with brands in my category?",
			answer: "We work with 7-8 figure Amazon brands across various categories. The strategies that drive profitable growth are universal, though we customize our approach for your specific business."
		},
		{
			question: "How do I get started with ALFI?",
			answer: "Book a strategy call to discuss your business goals and challenges. We'll assess if we're a good fit and outline a customized plan to grow your Amazon brand profitably."
		}
	];
</script>

<section class="py-24">
	<div class="mx-auto max-w-[1400px] px-6">
		<div class="grid grid-cols-1 gap-16 lg:grid-cols-12">
			<!-- Left Side -->
			<div class="lg:col-span-4">
				<div class="mb-4 text-[10px] font-bold tracking-widest text-gray-500 uppercase">[06] FAQ</div>
				<h2 class="mb-6 text-4xl font-medium tracking-tight text-gray-900">Your questions, answered</h2>
				<p class="mb-8 text-lg leading-relaxed text-gray-600">
					Ready to transform your Amazon brand into a profit engine? Book a strategy call to discuss your business and see if ALFI is the right fit.
				</p>
				<a href="#" class="inline-block bg-gray-900 px-6 py-3 text-[11px] font-bold tracking-widest text-white transition-colors hover:bg-gray-800 uppercase">
					Book Strategy Call
				</a>
			</div>

			<!-- Right Side (Accordion) -->
			<div class="lg:col-span-8">
				<div class="divide-y divide-gray-200 border-t border-b border-gray-200">
					{#each faqs as faq, i}
						<div class="group">
							<button 
								class="flex w-full items-center justify-between py-6 text-left focus:outline-none"
								onclick={() => openIndex = openIndex === i ? -1 : i}
							>
								<span class="text-lg font-medium text-gray-900">{faq.question}</span>
								<span class="ml-4 flex h-6 w-6 items-center justify-center text-gray-400">
									{#if openIndex === i}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 6L6 18M6 6l12 12"/></svg>
									{:else}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12h14"/></svg>
									{/if}
								</span>
							</button>
							{#if openIndex === i}
								<div class="pb-6 text-gray-600 leading-relaxed">
									{faq.answer}
								</div>
							{/if}
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
</section>