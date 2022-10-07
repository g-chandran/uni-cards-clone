<script lang="ts">
  import GradientText from "./GradientText.svelte";
</script>

<section
  class="h-[90vh] px-4 flex flex-col justify-end items-center gap-6 relative bg-[url(black_background_mobile.webp)] bg-cover"
>
  <img src="card_asset.webp" alt="BG" class="w-[255px] absolute top-[10rem]" />
  <p class="font-semibold text-white text-3xl mb-[9rem]">
    India’s Credit Revolution is here.
    <GradientText text="Pay 1/3rd" />
    Anywhere.
  </p>
</section>

<style>
  @keyframes up_down {
    from {
      transform: translateY(-3rem);
    }
    to {
      transform: translateY(1rem);
    }
  }
  img {
    animation-name: up_down;
    animation-duration: 5s;
    animation-iteration-count: infinite;
    animation-direction: alternate;
  }
</style>
