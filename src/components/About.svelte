<script>
    import "../routes/styles.css";


    import Icon from 'svelte-icon/Icon.svelte';
    import logo from '$lib/images/github.svg?raw';
  </script>
  
 

  <section class="text-gray-400 body-font lg:pt-40">
    <div class="container flex flex-wrap px-5 py-24 mx-auto items-center ">
      <div class="slide-left md:w-1/2 md:pr-12 md:py-8 md:border-r md:border-b-0 mb-10 md:mb-0 pb-10 border-b border-gray-200 pl-2">
        <h1 class="sm:text-x text-3xl l font-medium title-font mb-2 text-pink-500">Greetings, </h1>
        <p class="leading-relaxed text-2xl mb:text-lg">oh wanderer of the digital realm. I am Sanjana Bhat, an enigmatic frontend apprentice shrouded in the mysteries of the web. With a whisper of HTML and a flicker of CSS, I navigate the labyrinthine depths of code.</p>
  
      </div>
      <div class="flex flex-col mb:justify-center mb:align-center md:w-1/2 md:pl-12 slide-right">
        <h2 class="mb:ml-4 title-font font-semibold text-gray-500 tracking-wider text-2xl mb-3">Technologies I'm interested in and currently learning</h2>
        <nav class="flex flex-wrap justify-center items-center list-none -mb-1 mt-8 gap-0">
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-svelte glow-orange" title="Svelte"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-react glow-light-blue" title="React"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-html5 glow-red" title="HTML5"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-tailwindcss glow-medium-blue" title="TailwindCSS"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-nodejs glow-green" title="Node.js"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-javascript glow-yellow" title="JavaScript"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-python glow-light-blue" title="Python"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-git glow-orange" title="Git"></i>
          </li>
          <li class="lg:w-1/3 mb-1 w-1/2 text-center">
            <i class="lni lni-figma glow-purple" title="Figma"></i>
          </li>
        </nav>
      </div>
    </div>
  </section>
  
  <style>
    .lni {
      font-size: 48px;
      transition: all 0.3s ease;
    }
  
    li {
      margin-bottom: 20px;
    }
  
    .glow-orange:hover {
      text-shadow: 0 0 5px #ff7f00, 0 0 20px #ff7f00;
    }
    .glow-green:hover {
      text-shadow: 0 0 5px #679d5a, 0 0 20px #679d5a;
    }
  
    .glow-light-blue:hover {
      text-shadow: 0 0 5px #87ceeb, 0 0 20px #87ceeb;
    }
  
    .glow-medium-blue:hover {
      text-shadow: 0 0 5px #0000cd, 0 0 20px #0000cd;
    }
  
    .glow-yellow:hover {
      text-shadow: 0 0 5px #ffd700, 0 0 20px #ffd700;
    }

    .glow-red:hover {
      text-shadow: 0 0 5px #cf3d15, 0 0 20px #cf3d15;
    }

    .glow-purple:hover {
      text-shadow: 0 0 5px #5f2172, 0 0 20px #5f2172,  0 0 30px #5f2172;
    }

    @media (max-width: 768px) {
    .flex-wrap {
      justify-content: center;
    }
  }

  div {
    opacity: 0;
    animation: fade-in 1s ease-in forwards;
  }

  @keyframes fade-in {
    from{
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  .slide-left {
    animation: slide-l 1s ease-in forwards;
    opacity: 0;
  }

  @keyframes slide-l {
    from {
      transform: translateX(-100%);
      opacity: 0;
    }
    to {
      transform: translateX(0);
      opacity: 1;
    }
  }

  .slide-right {
    animation: slide-r 1s ease-in forwards;
    opacity: 0;
  }

  @keyframes slide-r {
    from {
      transform: translateX(100%);
      opacity: 0;
    }
    to {
      transform: translateX(0);
      opacity: 1;
    }
  }
  </style>

 