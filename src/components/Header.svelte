<script>
  import { onMount } from "svelte";

  let showMenu = false;

  function toggleNavbar() {
    showMenu = !showMenu;
  }

  function closeNavbar() {
    showMenu = false;
  }

  onMount(() => {
    document.body.addEventListener("click", function (event) {
      const header = document.querySelector("header");
      const isClickedOutsideHeader = !header.contains(event.target);
      if (isClickedOutsideHeader) {
        closeNavbar();
      }
    });
  });
</script>

<div>
  <div
    class="bg-transparent backdrop-blur-lg bg-opacity-0 fixed w-full z-20 top-0 left-0"
  >
    <nav
      class="container px-6 py-8 mx-auto md:flex md:justify-between md:items-center"
    >
      <div class="flex items-center justify-between lg:ml-10">
        <a href="/" class="flex items-center gap-2">
          <img src="/icon.svg" width="30px" height="30px" alt="" />
          <span
            class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
            >Sanjana</span
          >
        </a>

        <div on:click={toggleNavbar} class="flex md:hidden">
          <button
            type="button"
            class="text-gray-100 hover:text-gray-400 focus:outline-none focus:text-gray-400"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-6 h-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
              />
            </svg>
          </button>
        </div>
      </div>

      <div
        class="flex-col mr-10 mt-8 space-y-4  md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0  {showMenu
          ? 'flex'
          : 'hidden'}"
      >
        <a
          class="text-gray-100 hover:text-blue-400"
          on:click={closeNavbar}
          href="/">Home</a
        >
        <a
          class="text-gray-100 hover:text-blue-400"
          on:click={closeNavbar}
          href="/about">About Me</a
        >
        <a
          class="text-gray-100 hover:text-blue-400"
          on:click={closeNavbar}
          href="/projects">Projects</a
        >
        <a
          class="text-gray-100 hover:text-blue-400"
          on:click={closeNavbar}
          href="/photo">Gallery</a
        >
      </div>
    </nav>
  </div>
</div>
