<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section id="pricing" class="bg-[#f5f5f5] px-6 py-24 border-t border-gray-200">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Pricing" />
    </div>
    
    <div class="lg:col-span-9">
      <div class="mb-16">
        <h2 class="font-serif text-4xl md:text-5xl text-gray-900 mb-2">
          Start free, scale as you grow
        </h2>
        <h2 class="font-serif text-4xl md:text-5xl text-gray-400">
          20% off with annual billing
        </h2>
      </div>

      <div class="grid gap-0 border-t border-gray-200">
        <!-- Free Tier -->
        <a href="https://monitoring-spirit-frontend-2.pages.dev" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">$0/month</div>
            <h3 class="text-2xl font-medium text-gray-900">Free</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed mb-3">
              Perfect for individual validators getting started with on-chain monitoring.
            </p>
            <ul class="text-sm text-gray-600 space-y-1">
              <li>• 1 validator</li>
              <li>• 5-minute checks</li>
              <li>• Email notifications</li>
              <li>• 24-hour data retention</li>
            </ul>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>

        <!-- Pro Tier -->
        <a href="https://monitoring-spirit-frontend-2.pages.dev" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">$49/month</div>
            <h3 class="text-2xl font-medium text-gray-900">Pro</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed mb-3">
              For professional operators managing multiple validators with advanced alerting needs.
            </p>
            <ul class="text-sm text-gray-600 space-y-1">
              <li>• Up to 10 validators</li>
              <li>• 1-minute checks</li>
              <li>• Slack & Telegram alerts</li>
              <li>• 30-day retention</li>
              <li>• Performance benchmarking</li>
              <li>• Public status pages</li>
            </ul>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>

        <!-- Enterprise Tier -->
        <a href="mailto:support@roundbeat.io" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Custom pricing</div>
            <h3 class="text-2xl font-medium text-gray-900">Enterprise</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed mb-3">
              For exchanges, custodians, and large-scale operators requiring enterprise-grade reliability.
            </p>
            <ul class="text-sm text-gray-600 space-y-1">
              <li>• Unlimited validators</li>
              <li>• Real-time checks</li>
              <li>• PagerDuty integration</li>
              <li>• Unlimited webhooks</li>
              <li>• SSO support</li>
              <li>• 1-year retention</li>
              <li>• SLA guarantees</li>
            </ul>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>
      </div>
    </div>
  </div>
</section>
