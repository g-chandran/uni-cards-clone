<div class="mt-4 px-6">
  <div>
    <div class="font-semibold text-2xl text-gray-900 leading-10">
      <p>Split your payments,</p>
      <p>anywhere and everywhere.</p>
      <p class="text-gray-400">Accepted at 99.9% of merchants.</p>
    </div>
    <img class="my-10" src="backed_by_visa.svg" alt="backed by visa" />
  </div>
  <div class="relative overflow-hidden py-12 flex items-center">
    <img src="places.webp" alt="places" />
    <div
      class="circle-sun absolute top-3 left-6 -z-10 rounded-[150px_150px_0_0] w-[250px] h-[125px] bg-yellow-200"
    />
  </div>
</div>

<style>
  @keyframes up_down {
    from {
      transform: translateY(2rem);
    }
    to {
      transform: translateY(4rem);
    }
  }

  .circle-sun {
    animation-name: up_down;
    animation-duration: 4s;
    animation-iteration-count: infinite;
    animation-direction: alternate;
  }
</style>
