<script lang="ts">
  import GradientText from "../Components/GradientText.svelte";
  import SecondaryButton from "../Components/SecondaryButton.svelte";
</script>

<section
  class="bg-black p-4 h-[80vh] text-white flex flex-col gap-4 lg:flex-row lg:justify-center lg:items-center lg:gap-12"
>
  <div class="w-lg">
    <video
      muted
      playsinline
      disablepictureinpicture
      autoplay
      loop
      class="w-full h-full"
    >
      <source src="/one-third.mp4" type="video/mp4" /><source
        src="/videos/one-third.webm"
        type="video/webm"
      />
    </video>
  </div>
  <div class="flex flex-col gap-4 max-w-lg lg:gap-8">
    <h2 class="text-xl font-semibold lg:text-3xl">
      <GradientText text="Uni pay 1/3rd Card" />
    </h2>
    <p class="text-3xl font-bold lg:text-5xl lg:font-semibold">
      With Great Flexibility, Comes Great Power.
    </p>
    <p class="text-sm text-gray-400 lg:text-xl">
      Split your spends into
      <span class="text-white"> 3 parts over 3 months </span>
      at no extra charges. And,
      <span class="text-white"> get 1% rewards </span>
      if you pay in 1 month.
    </p>
    <span>
      <SecondaryButton title="Know More" />
    </span>
  </div>
</section>
