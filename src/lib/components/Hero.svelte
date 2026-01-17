<script lang="ts">
    import Navbar from './Navbar.svelte';
</script>

<section class="relative min-h-screen flex flex-col items-center pt-32 overflow-hidden bg-[#050505]">
    <!-- Gradient overlay to fade to black at bottom -->
    <div class="absolute inset-0 bg-[radial-gradient(circle_at_top,_var(--tw-gradient-stops))] from-primary-900/40 via-[#1a202c] to-[#050505] pointer-events-none opacity-80"></div>
    
    <Navbar transparent={true} />
    
    <div class="text-center z-10 px-4 max-w-4xl mx-auto mt-10">
        <div class="mb-6 text-white/80 text-sm font-medium tracking-widest uppercase">Setware by Ghoste</div>
        <h1 class="text-5xl md:text-7xl font-medium text-white tracking-tight mb-8 leading-[1.1]">
            Calm email for people<br />
            who do real work.
        </h1>
        
        <p class="text-white/60 text-lg md:text-xl max-w-2xl mx-auto mb-10">
            Setware helps you stay focused with automation-first email designed to reduce noise, not add to it. One-time setup. Lasting peace of mind.
        </p>

        <div class="flex items-center justify-center gap-6 mb-20">
            <a href="#waitlist" class="bg-primary-500 text-white px-8 py-4 rounded-full font-semibold hover:bg-primary-400 transition-colors shadow-lg shadow-primary-500/20">Join the waitlist</a>
            <span class="text-white/50 text-sm font-medium">Focus. Flow. Finish.</span>
        </div>
    </div>

    <!-- Hero Image -->
    <div class="relative w-full max-w-6xl mx-auto z-10 px-4">
        <div class="rounded-2xl overflow-hidden border border-white/10 shadow-2xl">
            <img 
                src="/generated/image-a-clean-minimalist-workspace-with-a-lapt-1768643224259-0.webp" 
                alt="Minimalist workspace" 
                class="w-full h-auto object-cover opacity-90"
            />
        </div>
        <!-- Fade out at bottom -->
        <div class="absolute bottom-0 left-0 right-0 h-32 bg-gradient-to-t from-[#050505] to-transparent"></div>
    </div>
</section>

<style>
    .perspective-2000 {
        perspective: 2000px;
    }
    .rotate-x-20 {
        transform: rotateX(20deg) rotateY(-10deg) rotateZ(5deg);
    }
</style>
