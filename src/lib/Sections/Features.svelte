<script lang="ts">
  import GradientText from "../Components/GradientText.svelte";
  import DownArrow from "virtual:icons/material-symbols/arrow-downward-rounded";
  import FeatureCard from "../Components/FeatureCard.svelte";
</script>

<section>
  <div
    class="max-w-7xl px-6 py-8 mx-auto text-gray-900 leading-10 font-semibold text-3xl lg:text-center lg:text-5xl"
  >
    <p>Split your payments, anywhere and everywhere.</p>
    <p>
      <GradientText text="Earn the best rewards." />
      Enjoy round the clock
      <GradientText text="WhatsApp support." /> It
    </p>
    <p>
      takes just 5 minutes to get your card, and it’s <GradientText
        text="lifetime free:"
      /> no joining fee, no annual charges.
    </p>
  </div>
  <div
    class="w-[96px] h-[96px] bg-gradient-to-tr from-green-400 to-yellow-400 flex justify-center items-center rounded-full my-12 mx-6"
  >
    <DownArrow style="font-size: 3rem" />
  </div>
  <ul>
    <FeatureCard />
  </ul>
</section>
