<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section id="features" class="bg-[#f5f5f5] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Why Roundbeat" />
    </div>
    
    <div class="lg:col-span-9 grid grid-cols-1 md:grid-cols-2 gap-16">
      <div>
        <h2 class="font-serif text-3xl md:text-4xl leading-tight text-gray-900 mb-6">
          See your validator health from the network's perspective, not just your node's
        </h2>
        <p class="text-gray-500 leading-relaxed">
          Pure on-chain monitoring that catches silent P2P failures and network partitions that local agents can't detect. Zero installation, zero maintenance.
        </p>
      </div>
      
      <div class="flex flex-col gap-8 pt-2">
        <div class="flex flex-col gap-2">
          <h3 class="text-sm font-medium text-gray-900">Network Consensus View</h3>
          <p class="text-xs text-gray-500 leading-relaxed">Monitors from outside-in, verifying what the network actually sees</p>
        </div>
        <div class="flex flex-col gap-2">
          <h3 class="text-sm font-medium text-gray-900">Zero Installation</h3>
          <p class="text-xs text-gray-500 leading-relaxed">No agents, no firewall configs, no maintenance burden</p>
        </div>
        <div class="flex flex-col gap-2">
          <h3 class="text-sm font-medium text-gray-900">Multi-Chain Ready</h3>
          <p class="text-xs text-gray-500 leading-relaxed">One platform for all your validators across different networks</p>
        </div>
      </div>
    </div>
  </div>
</section>
