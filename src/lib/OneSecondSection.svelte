<script lang="ts">
  import GradientText from "./GradientText.svelte";
  import SecondaryButton from "./SecondaryButton.svelte";
</script>

<section
  class="bg-black p-4 text-white flex flex-col gap-4 lg:flex-row lg:justify-center lg:items-center lg:gap-12"
>
  <div class="w-sm aspect-square">
    <video
      muted
      playsinline
      disablepictureinpicture
      autoplay
      loop
      class="w-full h-full"
    >
      <source src="/pay_half.mp4" type="video/mp4" /><source
        src="/pay_half.webm"
        type="video/webm"
      />
    </video>
  </div>
  <div class="flex flex-col gap-4 max-w-lg lg:gap-8">
    <h2 class="text-xl font-semibold lg:text-3xl">
      <GradientText text="Uni pay 1/2 Card" />
    </h2>
    <p class="text-3xl font-bold lg:text-5xl lg:font-semibold">
      Smart Payments, Delightful Rewards.
    </p>
    <p class="text-sm text-gray-400 lg:text-xl">
      <span class="text-white"> Split your spends in 2. </span>
      Or, pay in 1 month &
      <span class="text-white"> get 1.2% rewards! </span>
    </p>
    <span>
      <SecondaryButton title="Know More" />
    </span>
  </div>
</section>
