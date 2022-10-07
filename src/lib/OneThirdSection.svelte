<script lang="ts">
  import GradientText from "./GradientText.svelte";
  import SecondaryButton from "./SecondaryButton.svelte";
</script>

<section class="bg-black p-4 text-white flex flex-col gap-4">
  <video muted playsinline disablepictureinpicture class="w-full h-full">
    <source src="/one-third.mp4" type="video/mp4" /><source
      src="/videos/one-third.webm"
      type="video/webm"
    />
  </video>
  <h2 class="text-xl font-semibold">
    <GradientText text="Uni pay 1/3rd Card" />
  </h2>
  <p class="text-3xl font-bold">With Great Flexibility, Comes Great Power.</p>
  <p class="text-sm text-slate-500">
    Split your spends into
    <span class="text-white"> 3 parts over 3 months </span>
    at no extra charges. And,
    <span class="text-white"> get 1% rewards </span>
    if you pay in 1 month.
  </p>
  <span>
    <SecondaryButton title="Know More" />
  </span>
</section>
