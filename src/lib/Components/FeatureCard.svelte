<section>
  <!-- Split Payments -->
  <div
    class="mt-4 px-6 flex flex-col lg:flex-row w-full lg:items-center lg:justify-center lg:gap-16"
  >
    <div>
      <div
        class="font-semibold text-2xl text-gray-900 leading-10 lg:text-4xl max-w-xl"
      >
        <p>Split your payments,</p>
        <p>anywhere and everywhere.</p>
        <p class="text-gray-400">Accepted at 99.9% of merchants.</p>
      </div>
      <img class="my-10" src="backed_by_visa.svg" alt="backed by visa" />
    </div>
    <div class="relative overflow-hidden py-12 flex items-center max-w-xl">
      <img src="places.webp" alt="places" />
      <div
        class="circle-sun absolute top-3 left-6 -z-10 rounded-[150px_150px_0_0] w-[250px] h-[125px] bg-yellow-200 lg:w-[300px] lg:left-10 lg:h-[150px]"
      />
    </div>
  </div>
  <!-- Earn Rewards -->
  <div
    class="mt-4 px-6 flex flex-col lg:flex-row-reverse w-full lg:items-center lg:justify-center lg:gap-16"
  >
    <div>
      <div
        class="font-semibold text-2xl text-gray-900 leading-10 lg:text-4xl max-w-xl mb-16"
      >
        <p>Earn rewards every time</p>
        <p>you Pay in Full.</p>
        <p class="text-gray-400">Soon, get up to 5X value on Uni Store.</p>
      </div>
    </div>
    <div class="relative overflow-hidden py-12 flex items-center max-w-xl">
      <img src="reward_points.webp" alt="places" />
      <div
        class="circle-sun absolute top-10 left-3 -z-10 rounded-full w-[200px] h-[200px] bg-[rgb(122,255,236)] lg:w-[300px] lg:left-10 lg:h-[300px]"
      />
    </div>
  </div>
</section>

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
