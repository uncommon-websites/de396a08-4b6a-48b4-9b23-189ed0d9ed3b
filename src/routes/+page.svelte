<script lang="ts">
	import Hero from "$lib/components/Hero.svelte";
	import FeatureSection from "$lib/components/FeatureSection.svelte";
	import Footer from "$lib/components/Footer.svelte";
	
	import SplitInbox from "$lib/components/visuals/SplitInbox.svelte";
	import TextEditorSimple from "$lib/components/visuals/TextEditorSimple.svelte";
	import TextEditorToolbar from "$lib/components/visuals/TextEditorToolbar.svelte";
	import Speed from "$lib/components/visuals/Speed.svelte";
	import Design from "$lib/components/visuals/Design.svelte";
	import Keyboard from "$lib/components/visuals/Keyboard.svelte";
	import Security from "$lib/components/visuals/Security.svelte";
</script>

<main class="bg-ghoste-bg min-h-screen text-white selection:bg-primary-500/30">
	<Hero />
	
	<div class="mt-20 md:mt-40">
        <!-- Dark Mode Interface Section Divider -->
        <div class="px-4 max-w-6xl mx-auto mb-32 relative" id="philosophy">
             <div class="aspect-video bg-[#0A0A0A] rounded-lg border border-white/5 flex flex-col justify-end p-6 md:p-10 relative overflow-hidden">
                 <img src="/generated/image-an-abstract-serene-landscape-with-soft-g-1768643229005-2.webp" alt="Serene landscape" class="absolute inset-0 w-full h-full object-cover opacity-40" />
                 <div class="absolute inset-0 bg-gradient-to-b from-transparent to-black/80"></div>
                 <div class="relative z-10 flex flex-col gap-4">
                     <div class="flex items-center gap-2 text-white font-semibold">
                         <div class="w-4 h-4 bg-primary-500 rounded-full"></div> Ghoste Corp
                     </div>
                     <p class="text-2xl md:text-3xl font-medium text-white max-w-xl">
                        "Meaningful work happens in quiet, interruption-free spaces."
                     </p>
                 </div>
             </div>
             <div class="text-center mt-10 text-gray-500 text-sm flex flex-col items-center gap-2 cursor-pointer hover:text-white transition-colors">
                 <span class="transform rotate-90">›</span>
                 Discover the Ghoste philosophy.
             </div>
        </div>

		<FeatureSection 
            id="features"
			label="AUTOMATION-FIRST"
			title="Set it once. Forget the mess."
			description="Configure your inbox once, and let Setware handle the heavy lifting forever. Reclaim hours every week—and your sanity."
		>
			<div class="flex flex-col items-center gap-4">
                <div class="w-64 h-12 bg-white/5 border border-white/10 rounded-lg flex items-center px-4 gap-3 animate-pulse">
                    <div class="w-2 h-2 rounded-full bg-primary-500"></div>
                    <div class="h-2 w-32 bg-white/20 rounded"></div>
                </div>
                <div class="w-72 h-12 bg-white/5 border border-white/10 rounded-lg flex items-center px-4 gap-3">
                    <div class="w-2 h-2 rounded-full bg-primary-500"></div>
                    <div class="h-2 w-40 bg-white/20 rounded"></div>
                </div>
                <div class="w-64 h-12 bg-white/5 border border-white/10 rounded-lg flex items-center px-4 gap-3 animate-pulse delay-75">
                    <div class="w-2 h-2 rounded-full bg-primary-500"></div>
                    <div class="h-2 w-24 bg-white/20 rounded"></div>
                </div>
            </div>
		</FeatureSection>

		<FeatureSection 
			label="CHAT-LIKE THREADS"
			title="Email that feels like conversation."
			description="Setware transforms cluttered email chains into clean, chat-like threads. Read and reply with the speed of a messenger."
		>
			<div class="w-full max-w-md space-y-4">
                <div class="flex justify-start">
                    <div class="bg-white/5 border border-white/10 p-3 rounded-2xl rounded-bl-none max-w-[80%]">
                        <div class="h-2 w-32 bg-white/20 rounded mb-2"></div>
                        <div class="h-2 w-48 bg-white/10 rounded"></div>
                    </div>
                </div>
                <div class="flex justify-end">
                    <div class="bg-primary-500/20 border border-primary-500/30 p-3 rounded-2xl rounded-br-none max-w-[80%]">
                        <div class="h-2 w-40 bg-white/40 rounded"></div>
                    </div>
                </div>
            </div>
		</FeatureSection>

		<FeatureSection 
			label="SMART ORGANIZATION"
			title="No more inbox triage."
			description="Automatically sort, label, schedule, and respond—without lifting a finger after setup. Focus on the work, not the workflow."
		>
			<SplitInbox />
		</FeatureSection>

		<FeatureSection 
			label="UNMATCHED SPEED"
			title="Say goodbye to lag."
			description="With <50ms interactions, Setware delivers unmatched speed. Reach new heights with a new standard for responsiveness."
		>
			<Speed />
		</FeatureSection>

		<FeatureSection 
			label="QUIET DESIGN"
			title="Made for deep work."
			description="Designed to protect your attention with clean UI, zero distractions, and muted visual aesthetics. Generous whitespace for a clear mind."
		>
			<Design />
		</FeatureSection>

		<FeatureSection 
			label="POWER USER TOOLS"
			title="Built for your keyboard."
			description="Fly through your inbox with rapid-fire shortcuts for every action. Designed for developers and creators who value efficiency."
		>
			<Keyboard highlight="k" />
		</FeatureSection>

		<FeatureSection 
			label="PRIVACY FIRST"
			title="Your data stays yours."
			description="We don't store your emails or passwords. Setware integrates directly with Gmail and Outlook while respecting your privacy."
		>
			<Security />
		</FeatureSection>
	</div>

	<Footer />
</main>

