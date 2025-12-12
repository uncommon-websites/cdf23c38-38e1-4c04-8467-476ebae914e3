<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section class="bg-primary-50 px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Why Trust Us" />
    </div>
    
    <div class="lg:col-span-9 grid grid-cols-1 md:grid-cols-2 gap-16">
      <div>
        <h2 class="font-serif text-3xl md:text-4xl leading-tight text-primary-900 mb-6">
          The only crypto recovery service with public founders and proven security
        </h2>
        <p class="text-primary-700 leading-relaxed">
          We overcome industry distrust through transparency. Chris and Charles Brooks are publicly identified founders with media credibility and air-gapped infrastructure that keeps your data secure offline.
        </p>
      </div>
      
      <div class="flex gap-12 items-end pb-2">
        <div class="flex flex-col gap-1">
            <span class="text-4xl font-bold text-primary-900">55%</span>
            <span class="text-xs text-primary-500">Success Rate</span>
        </div>
        <div class="flex flex-col gap-1">
            <span class="text-4xl font-bold text-primary-900">$140B</span>
            <span class="text-xs text-primary-500">Locked Crypto Market</span>
        </div>
      </div>
    </div>
  </div>
</section>
