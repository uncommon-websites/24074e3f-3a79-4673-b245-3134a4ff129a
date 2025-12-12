<script lang="ts">
  import { slide } from 'svelte/transition';
  
  interface FAQItem {
    question: string;
    answer: string;
  }

  const faqs: FAQItem[] = [
    { question: "How does on-chain monitoring differ from local monitoring?", answer: "Local monitoring tools check your node from the inside-out, verifying that your software is running. Roundbeat monitors from the outside-in, checking what the network consensus actually sees. This catches silent P2P failures, network partitions, and other issues that your local node might not detect." },
    { question: "Do I need to install anything on my validator?", answer: "No. Roundbeat is completely agent-free. We connect directly to blockchain nodes and verify your validator's participation through on-chain consensus data. No installation, no firewall configuration, no maintenance required." },
    { question: "Which blockchains do you support?", answer: "We're currently live on Canton, Aztec, and Celestia networks. We're actively expanding to Ethereum, Cosmos Hub, Solana, Polygon, Avalanche, and Near. Each network integration tracks network-specific metrics like proof validity, topology sync, and data availability." },
    { question: "What happens when Roundbeat detects an issue?", answer: "You'll receive instant alerts through your preferred channels—email, Slack, Telegram, or PagerDuty for enterprise customers. Alerts include specific details about what the network is seeing, helping you diagnose issues faster." },
    { question: "Can I compare my validator's performance to others?", answer: "Yes. Pro and Enterprise tiers include benchmarking features that compare your validator's performance against the top 10% of the network, helping you identify optimization opportunities." },
    { question: "What's included in the free tier?", answer: "The free tier monitors 1 validator with 5-minute checks, email notifications, and 24-hour data retention. It's perfect for individual validators who want to try on-chain monitoring without commitment." },
    { question: "How do public status pages work?", answer: "Pro and Enterprise customers can create public status pages that prove validator reliability to delegators. These pages show uptime metrics and performance data, building trust with your community." }
  ];

  let openIndex: number | null = null;

  function toggle(index: number) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section class="bg-[#f5f5f5] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-4">
      <h2 class="font-serif text-4xl text-gray-900 mb-6">
        Frequently asked questions
      </h2>
      <a href="mailto:support@roundbeat.io" class="text-sm text-gray-900 border-b border-gray-300 pb-0.5 hover:border-black transition-colors">Contact support</a>
    </div>
    
    <div class="lg:col-span-8">
      <div class="border-t border-gray-200">
        {#each faqs as faq, i}
          <div class="border-b border-gray-200">
            <button 
              class="w-full py-6 flex justify-between items-center text-left hover:bg-gray-50 transition-colors"
              on:click={() => toggle(i)}
            >
              <span class="text-lg text-gray-800">{faq.question}</span>
              <span class="text-2xl font-light text-gray-400 ml-4">
                {openIndex === i ? '−' : '+'}
              </span>
            </button>
            {#if openIndex === i}
              <div transition:slide class="pb-6 text-gray-500 leading-relaxed">
                {faq.answer}
              </div>
            {/if}
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
