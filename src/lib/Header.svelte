<script lang="ts">
  import Menu from "virtual:icons/material-symbols/menu";
  import Close from "virtual:icons/material-symbols/close";
  import RightArrow from "virtual:icons/material-symbols/arrow-forward-rounded";
  import { slide } from "svelte/transition";
  import { cubicInOut } from "svelte/easing";
  $: isOpen = false;
</script>

<header class="relative">
  <nav
    class="bg-black max-w-lg flex flex-row justify-between py-5 px-6 items-start"
  >
    <span class="w-12 h-12 text-white mt-[-15px]">
      <svg
        class="w-[100px] h-[80px]"
        viewBox="0 0 85 60"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        ><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M54.894 39.5039H48.6641V19.77H54.894V39.5039ZM30.4021 25.9999V39.504H24.1723V22.3647C24.1723 21.6765 24.4457 21.0165 24.9322 20.5301C25.4188 20.0435 26.0787 19.77 26.7669 19.77H42.3312C43.0195 19.77 43.6793 20.0435 44.1657 20.5301C44.6523 21.0165 44.9257 21.6765 44.9257 22.3647V39.504H38.696V25.9999H30.4021ZM14.2345 33.2742V19.7702H20.4644V36.9095C20.4644 37.5977 20.1909 38.2576 19.7044 38.744C19.2179 39.2307 18.5579 39.5041 17.87 39.5041H2.30544C1.61752 39.5041 0.957379 39.2307 0.470894 38.744C-0.0157201 38.2576 -0.289062 37.5977 -0.289062 36.9095V19.7702H5.9407V33.2742H14.2345Z"
          fill="white"
        /><path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M65.289 19.7708C65.289 21.8685 63.5858 23.5717 61.4882 23.5717C59.3905 23.5717 57.6875 21.8685 57.6875 19.7708C57.6875 17.6732 59.3905 15.9702 61.4882 15.9702C63.5858 15.9702 65.289 17.6732 65.289 19.7708Z"
          fill="#00DCC8"
        /></svg
      >
    </span>
    <span on:click={() => (isOpen = !isOpen)} class="text-white lg:hidden">
      {#if isOpen}
        <Close style="font-size: 2em" />
      {:else}
        <Menu style="font-size: 2em" />
      {/if}
    </span>
    <div class="text-white hidden lg:visible">
      <a href="/">Pay 1/3rd Card</a>
      <a href="/">Pay 1/2 Card</a>
    </div>
  </nav>
  {#if isOpen}
    <ul
      transition:slide={{ easing: cubicInOut, duration: 200 }}
      class="text-white absolute w-full flex flex-col pb-4 font-semibold border-t border-t-white bg-black bg-opacity-90"
    >
      <li class="flex justify-between items-center py-4 px-6 border-b">
        <a href="/">Pay 1/3rd Card</a>
        <RightArrow style="font-size: 1.5rem" />
      </li>
      <li class="flex justify-between items-center py-2 px-6">
        <a href="/">Pay 1/2 Card</a>
        <RightArrow style="font-size: 1.5rem" />
      </li>
    </ul>
  {/if}
</header>
