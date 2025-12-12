<script>
  import Navbar from '$lib/components/Navbar.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import Logos from '$lib/components/Logos.svelte';
  import WhyRoundbeat from '$lib/components/WhyRoundbeat.svelte';
  import Products from '$lib/components/Products.svelte';
  import Founders from '$lib/components/Founders.svelte';
  import FAQ from '$lib/components/FAQ.svelte';
  import BottomCTA from '$lib/components/BottomCTA.svelte';
  import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
  <title>Roundbeat - Objective Validator Health Monitoring</title>
  <meta name="description" content="Zero-installation blockchain validator monitoring via on-chain consensus verification. Catch network-level failures that local tools miss." />
</svelte:head>

<div class="min-h-screen bg-[#f5f5f5] font-sans selection:bg-black selection:text-white">
  <Navbar />
  <Hero />
  <Logos />
  <WhyRoundbeat />
  <Products />
  <Founders />
  <FAQ />
  <BottomCTA />
  <Footer />
</div>

