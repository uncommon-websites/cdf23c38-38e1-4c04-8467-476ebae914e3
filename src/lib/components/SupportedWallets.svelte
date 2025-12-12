<script lang="ts">
  import SectionLabel from './SectionLabel.svelte';
</script>

<section id="supported-wallets" class="bg-white px-6 py-24 border-t border-primary-100">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Supported Wallets" />
    </div>
    
    <div class="lg:col-span-9">
      <div class="mb-16">
        <h2 class="font-serif text-4xl md:text-5xl text-primary-900 mb-4">
          We work with the wallets you use
        </h2>
        <p class="text-primary-700 text-lg leading-relaxed max-w-2xl">
          Whether you've been using crypto for years or just getting started, we can help recover access to your wallet. Here are some of the most common wallets we support.
        </p>
      </div>

      <!-- Wallet Grid -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-12">
        <!-- Blockchain.com -->
        <div class="border border-primary-200 p-6 rounded hover:border-primary-300 transition-colors">
          <div class="flex items-start gap-4">
            <div class="w-12 h-12 bg-white border-2 border-primary-200 rounded flex items-center justify-center flex-shrink-0 overflow-hidden">
              <img src="https://logo.clearbit.com/blockchain.com" alt="Blockchain.com logo" class="w-8 h-8 object-contain" />
            </div>
            <div>
              <h3 class="text-xl font-medium text-primary-900 mb-2">Blockchain.com</h3>
              <p class="text-sm text-primary-600 leading-relaxed">
                One of the most popular online wallets. We can help if you've forgotten your password or lost access to your account.
              </p>
            </div>
          </div>
        </div>

        <!-- Bitcoin Core -->
        <div class="border border-primary-200 p-6 rounded hover:border-primary-300 transition-colors">
          <div class="flex items-start gap-4">
            <div class="w-12 h-12 bg-white border-2 border-primary-200 rounded flex items-center justify-center flex-shrink-0 overflow-hidden">
              <img src="https://logo.clearbit.com/bitcoin.org" alt="Bitcoin Core logo" class="w-8 h-8 object-contain" />
            </div>
            <div>
              <h3 class="text-xl font-medium text-primary-900 mb-2">Bitcoin Core</h3>
              <p class="text-sm text-primary-600 leading-relaxed">
                The original Bitcoin wallet software. We specialize in recovering older Bitcoin Core wallets with forgotten passwords.
              </p>
            </div>
          </div>
        </div>

        <!-- MetaMask -->
        <div class="border border-primary-200 p-6 rounded hover:border-primary-300 transition-colors">
          <div class="flex items-start gap-4">
            <div class="w-12 h-12 bg-white border-2 border-primary-200 rounded flex items-center justify-center flex-shrink-0 overflow-hidden">
              <img src="https://logo.clearbit.com/metamask.io" alt="MetaMask logo" class="w-8 h-8 object-contain" />
            </div>
            <div>
              <h3 class="text-xl font-medium text-primary-900 mb-2">MetaMask</h3>
              <p class="text-sm text-primary-600 leading-relaxed">
                Popular browser extension for Ethereum and NFTs. We can help recover access if you've lost your password or seed phrase.
              </p>
            </div>
          </div>
        </div>

        <!-- Trust Wallet -->
        <div class="border border-primary-200 p-6 rounded hover:border-primary-300 transition-colors">
          <div class="flex items-start gap-4">
            <div class="w-12 h-12 bg-white border-2 border-primary-200 rounded flex items-center justify-center flex-shrink-0 overflow-hidden">
              <img src="https://logo.clearbit.com/trustwallet.com" alt="Trust Wallet logo" class="w-8 h-8 object-contain" />
            </div>
            <div>
              <h3 class="text-xl font-medium text-primary-900 mb-2">Trust Wallet</h3>
              <p class="text-sm text-primary-600 leading-relaxed">
                Mobile wallet for multiple cryptocurrencies. We can assist with password recovery and seed phrase issues.
              </p>
            </div>
          </div>
        </div>

        <!-- Electrum -->
        <div class="border border-primary-200 p-6 rounded hover:border-primary-300 transition-colors">
          <div class="flex items-start gap-4">
            <div class="w-12 h-12 bg-white border-2 border-primary-200 rounded flex items-center justify-center flex-shrink-0 overflow-hidden">
              <img src="https://logo.clearbit.com/electrum.org" alt="Electrum logo" class="w-8 h-8 object-contain" />
            </div>
            <div>
              <h3 class="text-xl font-medium text-primary-900 mb-2">Electrum</h3>
              <p class="text-sm text-primary-600 leading-relaxed">
                Lightweight Bitcoin wallet known for speed and security. We have extensive experience with Electrum recovery.
              </p>
            </div>
          </div>
        </div>

        <!-- MyEtherWallet -->
        <div class="border border-primary-200 p-6 rounded hover:border-primary-300 transition-colors">
          <div class="flex items-start gap-4">
            <div class="w-12 h-12 bg-white border-2 border-primary-200 rounded flex items-center justify-center flex-shrink-0 overflow-hidden">
              <img src="https://logo.clearbit.com/myetherwallet.com" alt="MyEtherWallet logo" class="w-8 h-8 object-contain" />
            </div>
            <div>
              <h3 class="text-xl font-medium text-primary-900 mb-2">MyEtherWallet</h3>
              <p class="text-sm text-primary-600 leading-relaxed">
                Free, open-source interface for Ethereum. We can help recover access to your MEW wallet and tokens.
              </p>
            </div>
          </div>
        </div>
      </div>

      <!-- Additional Support Info -->
      <div class="bg-primary-50 border border-primary-200 p-8 rounded">
        <h3 class="text-lg font-medium text-primary-900 mb-4">And many more wallets</h3>
        <div class="grid md:grid-cols-2 gap-4 mb-6">
          <div class="flex items-start gap-2">
            <span class="text-primary-500 flex-shrink-0">✓</span>
            <span class="text-sm text-primary-700">Multibit and Multibit HD</span>
          </div>
          <div class="flex items-start gap-2">
            <span class="text-primary-500 flex-shrink-0">✓</span>
            <span class="text-sm text-primary-700">Dogechain wallets</span>
          </div>
          <div class="flex items-start gap-2">
            <span class="text-primary-500 flex-shrink-0">✓</span>
            <span class="text-sm text-primary-700">Mist Ethereum Wallet</span>
          </div>
          <div class="flex items-start gap-2">
            <span class="text-primary-500 flex-shrink-0">✓</span>
            <span class="text-sm text-primary-700">Hardware wallet backups</span>
          </div>
        </div>
        <p class="text-sm text-primary-600 leading-relaxed">
          Don't see your wallet listed? We're constantly adding support for new wallets and cryptocurrencies. <a href="#contact" class="text-primary-900 border-b border-gray-300 hover:border-primary-700 transition-colors">Get in touch</a> and we'll let you know if we can help.
        </p>
      </div>
    </div>
  </div>
</section>
