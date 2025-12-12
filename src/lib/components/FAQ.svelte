<script lang="ts">
  import { slide } from 'svelte/transition';
  
  interface FAQItem {
    question: string;
    answer: string;
  }

  const faqs: FAQItem[] = [
    { 
      question: "How secure is your recovery process?", 
      answer: "All wallet recovery happens on air-gapped servers—completely offline with no internet connection. Your data is encrypted in transit and at rest. We never request your full password, and you control what information you share with us. Our infrastructure uses custom password cracking servers with Cloudflare security integration." 
    },
    { 
      question: "What is your success rate?", 
      answer: "We maintain a 55% success rate, which is industry-leading. Recovery time ranges from 1 hour to 6+ months depending on complexity. Initial searches are typically exhausted within one week, and we continue retesting as new recovery vectors are discovered." 
    },
    { 
      question: "What cryptocurrencies and wallets do you support?", 
      answer: "We support Bitcoin, Ethereum, Litecoin, Dogecoin, NFTs, and dozens of altcoins. Wallet support includes Blockchain.com, Bitcoin Core, Multibit, Electrum, MetaMask, MyEtherWallet, Mist Ethereum Wallet, Dogechain Core, and more. We're expanding supported cryptocurrencies daily." 
    },
    { 
      question: "How much does wallet recovery cost?", 
      answer: "We operate on a no recovery, no fee model—completely risk-free. You only pay if we successfully recover your wallet. This means there's no upfront cost or financial risk to you. We help anyone regardless of wallet size, unlike competitors who prioritize only the largest cases." 
    },
    { 
      question: "Why should I trust you over other recovery services?", 
      answer: "We're the only crypto asset recovery company with public founders. Chris and Charles Brooks are fully identified with disclosed backgrounds. We've been featured in 100+ publications including BBC, Forbes, VICE, and The Block. We're a registered LLC in New Hampshire with a public business address. Dozens of impersonator companies exist—we're the only legitimate service with a doxxed team." 
    },
    { 
      question: "How long does the recovery process take?", 
      answer: "Recovery timelines vary from 1 hour to 6+ months depending on password complexity and wallet type. Most initial searches are completed within one week. We continuously expand our hardware capabilities and retest wallets as new recovery techniques are discovered, so even if initial attempts fail, we may succeed later." 
    },
    { 
      question: "Do you offer services beyond wallet recovery?", 
      answer: "Yes, we offer scam tracing services starting at $475. This includes blockchain analysis of up to 50 transactions and investigation reports for law enforcement. We help build cases for criminal and civil legal proceedings. Note that this is investigation only, not a recovery service. Free consultation available for scam cases." 
    }
  ];

  let openIndex: number | null = null;

  function toggle(index: number) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section id="faq" class="bg-[#f5f5f5] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-4">
      <h2 class="font-serif text-4xl text-gray-900 mb-6">
        Frequently asked questions
      </h2>
      <a href="#contact" class="text-sm text-gray-900 border-b border-gray-300 pb-0.5 hover:border-black transition-colors">Get in touch</a>
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
