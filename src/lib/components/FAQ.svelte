<script lang="ts">
  import { slide } from 'svelte/transition';
  
  interface FAQItem {
    question: string;
    answer: string;
  }

  const faqs: FAQItem[] = [
    { 
      question: "Is my information safe with you?", 
      answer: "Absolutely. All wallet recovery happens on computers that are completely disconnected from the internet—no one can access them remotely. Your information is encrypted and secure. We never ask for your full password, and you decide what details to share with us. Your security is our top priority." 
    },
    { 
      question: "What are my chances of getting my wallet back?", 
      answer: "We've successfully recovered over 55% of the wallets we've worked on. How long it takes depends on your specific situation—some cases are resolved in hours, others take several months. Most people hear back from us within the first week. Even if we can't recover your wallet right away, we keep trying as we develop new techniques." 
    },
    { 
      question: "Which wallets can you help with?", 
      answer: "We work with all the major wallets including Blockchain.com, Bitcoin Core, MetaMask, Trust Wallet, Electrum, MyEtherWallet, and many others. We support Bitcoin, Ethereum, Litecoin, Dogecoin, NFTs, and dozens of other cryptocurrencies. If you're not sure whether we can help with your specific wallet, just reach out and ask—we're happy to let you know." 
    },
    { 
      question: "How much does this cost?", 
      answer: "You only pay if we successfully recover your wallet. There's no upfront cost and no risk to you. We help everyone, whether your wallet has a little or a lot in it. Many other recovery services only take the biggest cases, but we believe everyone deserves help getting their crypto back." 
    },
    { 
      question: "How do I know you're legitimate?", 
      answer: "We're a real family business run by Chris and Charles Brooks, a father and son team. Unlike other recovery services, we use our real names and show our faces. We've been featured in major publications like BBC, Forbes, and VICE. We're a registered business in New Hampshire with a real address. Unfortunately, there are fake companies pretending to be us, so always make sure you're contacting the real Crypto Asset Recovery." 
    },
    { 
      question: "How long will it take?", 
      answer: "It varies quite a bit depending on your situation. Some wallets we can recover in just a few hours, while others might take several months. The good news is that most people hear back from us within the first week with an initial update. We keep working on your case over time, and sometimes we succeed months later using new recovery methods we've developed." 
    },
    { 
      question: "Can you help if I was scammed?", 
      answer: "If your crypto was stolen or you were scammed, we can help trace where it went. This service starts at $475 and includes tracking up to 50 transactions and creating a detailed report for law enforcement. While we can't get stolen funds back, we can help you build a case for legal action. We offer a free consultation to discuss your situation and see if we can help." 
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
        Common questions
      </h2>
      <p class="text-gray-500 mb-4 leading-relaxed">Still have questions? We're here to help.</p>
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
