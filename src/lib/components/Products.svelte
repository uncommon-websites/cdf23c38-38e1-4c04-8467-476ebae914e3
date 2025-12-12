<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section id="services" class="bg-[#f5f5f5] px-6 py-24 border-t border-gray-200">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Our Services" />
    </div>
    
    <div class="lg:col-span-9">
      <div class="mb-16">
        <h2 class="font-serif text-4xl md:text-5xl text-gray-900 mb-2">
          Wallet Recovery
        </h2>
        <h2 class="font-serif text-4xl md:text-5xl text-gray-400">
          and Scam Tracing
        </h2>
      </div>

      <div class="grid gap-0 border-t border-gray-200">
        <!-- Item 1 -->
        <a href="#contact" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">No recovery, no fee</div>
            <h3 class="text-2xl font-medium text-gray-900">Crypto Wallet Recovery</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed mb-3">
              Recover access to locked Bitcoin, Ethereum, Litecoin, Dogecoin wallets and NFTs. Our air-gapped password cracking servers test billions to trillions of combinations to restore your wallet access. Supports Blockchain.com, Bitcoin Core, MetaMask, Electrum, and more.
            </p>
            <p class="text-xs text-gray-400">
              Timeline: 1 hour to 6+ months • Success rate: 55%
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>

        <!-- Item 2 -->
        <a href="#contact" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-gray-200 hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Starting at $475</div>
            <h3 class="text-2xl font-medium text-gray-900">Scam Tracing</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-500 leading-relaxed mb-3">
              Blockchain analysis and investigation reports for law enforcement. We trace up to 50 transactions and provide detailed event reporting to help build cases for criminal and civil legal proceedings. Free consultation available.
            </p>
            <p class="text-xs text-gray-400">
              Note: Investigation only, not recovery service
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-black transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>
      </div>
    </div>
  </div>
</section>
