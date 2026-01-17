<script lang="ts">
  type Props = {
    transparent?: boolean;
  };
  let { transparent = false }: Props = $props();
</script>

<nav class="fixed top-0 left-0 right-0 z-50 flex items-center justify-between px-6 py-6 transition-colors duration-300 {transparent ? 'bg-transparent' : 'bg-ghoste-bg/80 backdrop-blur-md'}">
  <div class="flex-1">
    <a href="/" class="text-white font-bold tracking-tighter text-xl">Ghoste</a>
  </div>
  
  <div class="hidden md:block text-xs font-medium text-white/60 tracking-wide absolute left-1/2 transform -translate-x-1/2 uppercase">
    Focus. Flow. Finish.
  </div>

  <div class="flex items-center gap-6 text-xs font-medium text-white/70">
    <a href="#features" class="hover:text-white transition-colors">Features</a>
    <a href="#philosophy" class="hover:text-white transition-colors">Philosophy</a>
    <a href="#waitlist" class="text-white hover:text-primary-400 transition-colors">Join Waitlist</a>
  </div>
</nav>
