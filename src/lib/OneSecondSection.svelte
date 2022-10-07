<script lang="ts">
  import GradientText from "./GradientText.svelte";
  import SecondaryButton from "./SecondaryButton.svelte";
</script>

<section class="bg-black p-4 text-white flex flex-col gap-4 mt-[-1px]">
  <video
    muted={true}
    playsinline={true}
    disablepictureinpicture={true}
    class="w-full h-full"
  >
    <source src="/pay_half.mp4" type="video/mp4" /><source
      src="/one-third.webm"
      type="video/webm"
    />
  </video>
  <h2 class="text-xl font-semibold">
    <GradientText text="Uni pay 1/2 Card" />
  </h2>
  <p class="text-3xl font-bold">Smart Payments, Delightful Rewards.</p>
  <p class="text-sm text-slate-500">
    <span class="text-white"> Split your spends in 2. </span>
    Or, pay in 1 month &
    <span class="text-white"> get 1.2% rewards! </span>
  </p>
  <span>
    <SecondaryButton title="Know More" />
  </span>
</section>
