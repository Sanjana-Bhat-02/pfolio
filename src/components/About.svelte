<script>
  import "../routes/styles.css";
  import "../routes/glow.css";
  import { LottiePlayer } from "@lottiefiles/svelte-lottie-player";

  let controlsLayout = [
    "previousFrame",
    "playpause",
    "stop",
    "nextFrame",
    "progress",
    "frame",
    "loop",
    "spacer",
    "background",
    "snapshot",
    "zoom",
    "info",
  ];
</script>

<section class="text-gray-400 body-font lg:pt-40">
  <div class="container flex flex-wrap px-5 py-24 mx-auto items-center">
    <div
      class="slide-left md:w-1/2 md:pr-12 md:py-8 md:border-r md:border-b-0 mb-10 md:mb-0 pb-10 border-b border-gray-200 pl-2"
    >
      <h1
        class="sm:text-x text-3xl l font-medium title-font mb-2 text-pink-500"
      >
        Greetings,
      </h1>
      <p class="leading-relaxed text-2xl mb:text-lg">
        oh wanderer of the digital realm. I am Sanjana Bhat, an enigmatic
        frontend apprentice shrouded in the mysteries of the web. With a whisper
        of HTML and a flicker of CSS, I navigate the intricate depths of code.
      </p>
    </div>
    <div
      class="flex flex-col mb:justify-center mb:align-center md:w-1/2 md:pl-12 slide-right"
    >
      <h2
        class="mb:ml-4 title-font font-semibold text-gray-500 tracking-wider text-2xl mb-3"
      >
        Technologies I'm interested in and currently learning
      </h2>
      <nav
        class="flex flex-wrap justify-center items-center list-none -mb-1 mt-8 gap-0"
      >
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-svelte glow-orange" title="Svelte" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-react glow-light-blue" title="React" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-html5 glow-red" title="HTML5" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-tailwindcss glow-medium-blue" title="TailwindCSS" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-nodejs glow-green" title="Node.js" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-javascript glow-yellow" title="JavaScript" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-python glow-light-blue" title="Python" />
        </li>
        <li class="lg:w-1/3 mb-1 w-1/2 text-center">
          <i class="lni lni-git glow-orange" title="Git" />
        </li>
      </nav>
    </div>
  </div>
</section>

<h1 class="text-pink-500 text-center text-4xl mt-10">My Interests</h1>
<section class="text-gray-600 body-font mb-20">
  <div class="container px-5 py-24 mx-auto">
    <div
      class="flex items-center lg:w-3/5 mx-auto border-b pb-10 mb-10 border-gray-200 sm:flex-row flex-col"
    >
      <div
        class="sm:w-32 sm:h-32 h-20 w-20 sm:mr-10 inline-flex items-center justify-center rounded-full bg-gray-400 text-slate-950 flex-shrink-0"
      >
        <i class="lni lni-book" />
      </div>
      <div class="flex-grow sm:text-left text-center mt-6 sm:mt-0">
        <h2 class="text-blue-400 text-2xl title-font font-medium mb-2">
          Reading Books
        </h2>
        <p class="leading-relaxed text-base text-gray-400 text-xl">
          Getting lost in stories, learning new things, and expanding my
          imagination with every turn of the page.
        </p>
      </div>
    </div>
    <div
      class="flex items-center lg:w-3/5 mx-auto border-b pb-10 mb-10 border-gray-200 sm:flex-row flex-col"
    >
      <div class="flex-grow sm:text-left text-center mt-6 sm:mt-0">
        <h2 class="text-blue-400 text-2xl title-font font-medium mb-2">
          Drawing & Painting
        </h2>
        <p class="leading-relaxed text-base text-gray-400 text-xl">
          Using colors and brushes, I express my feelings, ideas, and creativity
          on a canvas, bringing art to life.
        </p>
      </div>
      <div
        class="sm:w-32 sm:order-none order-first sm:h-32 h-20 w-20 sm:ml-10 inline-flex items-center justify-center rounded-full bg-gray-400 text-slate-950 flex-shrink-0"
      >
        <i class="lni lni-brush-alt" />
      </div>
    </div>
    <div class="flex items-center lg:w-3/5 mx-auto sm:flex-row flex-col">
      <div
        class="sm:w-32 sm:h-32 h-20 w-20 sm:mr-10 inline-flex items-center justify-center rounded-full bg-gray-400 text-slate-950 flex-shrink-0"
      >
        <i class="lni lni-camera" />
      </div>
      <div class="flex-grow sm:text-left text-center mt-6 sm:mt-0">
        <h2 class="text-blue-400 text-2xl title-font font-medium mb-2">
          Photography
        </h2>
        <p class="leading-relaxed text-base text-gray-400 text-xl">
          With my camera in hand, I capture moments, freeze memories, and tell
          stories through the snapshots I take.
        </p>
        <a href="/photo" class="mt-3 text-indigo-500 inline-flex items-center"
          >Go to Gallery
          <svg
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            class="w-4 h-4 ml-2"
            viewBox="0 0 24 24"
          >
            <path d="M5 12h14M12 5l7 7-7 7" />
          </svg>
        </a>
      </div>
    </div>
  </div>
</section>

<h1 class="text-pink-500 text-center text-4xl mt-10">Education</h1>
<section class="text-gray-600 body-font ml-20 pt-0">
  <div class="container px-5 mx-auto flex flex-wrap">
    <div class="flex flex-wrap w-full">
      <div class="lg:w-2/5 md:w-1/2 md:pr-10 md:py-6 mt-24">
        <div class="flex relative pb-12">
          <div
            class="h-full w-10 absolute inset-0 flex items-center justify-center"
          >
            <div class="h-full w-1 bg-gray-200 pointer-events-none" />
          </div>
          <div
            class="flex-shrink-0 w-10 h-10 rounded-full bg-gray-400 inline-flex items-center justify-center text-white relative z-10"
          >
            <!-- Generator: Adobe Illustrator 22.0.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
            <svg
              fill="#1C2033"
              width="25"
              height="25"
              version="1.1"
              id="lni_lni-pencil"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              x="0px"
              y="0px"
              viewBox="0 0 64 64"
              style="enable-background:new 0 0 64 64;"
              xml:space="preserve"
            >
              <path
                d="M61.2,13c-3.2-3.4-6.6-6.8-10-10.1c-0.7-0.7-1.5-1.1-2.4-1.1c-0.9,0-1.8,0.3-2.4,1L8.7,40.2c-0.6,0.6-1,1.3-1.3,2L1.9,59
	c-0.3,0.8-0.1,1.6,0.3,2.2c0.5,0.6,1.2,1,2.1,1h0.4l17.1-5.7c0.8-0.3,1.5-0.7,2-1.3l37.5-37.4c0.6-0.6,1-1.5,1-2.4
	S61.9,13.7,61.2,13z M20.6,52.1c-0.1,0.1-0.2,0.1-0.3,0.2L7.4,56.6l4.3-12.9c0-0.1,0.1-0.2,0.2-0.3L39.4,16l8.7,8.7L20.6,52.1z
	 M51.2,21.5l-8.7-8.7l6.1-6.1c2.9,2.8,5.8,5.8,8.6,8.7L51.2,21.5z"
              />
            </svg>
          </div>
          <div class="flex-grow pl-4">
            <h2
              class="font-medium title-font text-2xl text-blue-400 mb-1 tracking-wider"
            >
              SSLC - 10th Std
            </h2>
            <p class="leading-relaxed text-gray-300 text-lg">
              Jaimatha Senior Secondary School, Kasaragod, Kerala
            </p>
          </div>
        </div>

        <div class="flex relative pb-12">
          <div
            class="h-full w-10 absolute inset-0 flex items-center justify-center"
          >
            <div class="h-full w-1 bg-gray-200 pointer-events-none" />
          </div>
          <div
            class="flex-shrink-0 w-10 h-10 rounded-full bg-gray-400 inline-flex items-center justify-center text-white relative z-10"
          >
            <!-- Generator: Adobe Illustrator 22.0.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->

            <svg
              fill="#1C2033"
              width="25"
              height="25"
              version="1.1"
              id="lni_lni-cogs"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              x="0px"
              y="0px"
              viewBox="0 0 64 64"
              style="enable-background:new 0 0 64 64;"
              xml:space="preserve"
            >
              <g>
                <path
                  d="M43,34.1c-4.8,0-8.8,4-8.8,8.8s3.9,8.8,8.8,8.8s8.8-4,8.8-8.8S47.8,34.1,43,34.1z M43,47.3c-2.4,0-4.3-1.9-4.3-4.3
 c0-2.4,1.9-4.3,4.3-4.3s4.3,1.9,4.3,4.3C47.3,45.3,45.4,47.3,43,47.3z"
                />
                <path
                  d="M61.8,46.2l-3.1-1.7c0.1-0.6,0.1-1.2,0.1-1.7c0-0.6,0-1.2-0.1-1.7l3.2-1.8c1.2-0.7,1.6-2.1,1.1-3.4l-3.8-6.5
 c-0.7-1.1-2.1-1.6-3.3-1.1l-3.5,1.9c0,0-0.1-0.1-0.1-0.1c-0.6-0.5-1.3-1.1-2.2-1.6v-2.1c0-2.1-1.7-3.9-3.9-3.9h-6.5
 c-2.1,0-3.9,1.7-3.9,3.9v2.1c-0.9,0.5-1.6,1.1-2.3,1.6c0,0,0,0,0,0l-2.9-1.6c-1.8-1-3.3-0.3-3.9,0.8l-3.6,6.1
 c-0.4,0.6-0.5,1.4-0.3,2.1c0.2,0.7,0.7,1.3,1.3,1.6l3.2,1.7c-0.1,0.5-0.1,1.1-0.1,1.7c0,0.6,0,1.1,0.1,1.7L24,46.3
 c-1.2,0.7-1.6,2.1-1.1,3.4l3.8,6.5c0.7,1.1,2.1,1.6,3.3,1.1l3.5-1.9c0,0,0.1,0,0.1,0.1c0.7,0.6,1.3,1.1,2.3,1.6v2.4
 c0,2.1,1.7,3.9,3.9,3.9h6.5c2.1,0,3.9-1.7,3.9-3.9v-2.5c0.9-0.5,1.5-1,2.2-1.6c0,0,0.1,0,0.1-0.1l2.9,1.6c1.8,1,3.3,0.3,3.9-0.8
 l3.6-6.1c0.4-0.6,0.5-1.4,0.3-2.1C62.9,47.1,62.5,46.5,61.8,46.2z M54.2,41c0.1,0.5,0.1,1.1,0.1,1.8c0,0.6,0,1.2-0.2,1.8
 c-0.2,1.4,0.4,2.8,1.7,3.5l2.2,1.2l-1.8,3l-2.4-1.4c-1.2-0.7-2.6-0.5-3.6,0.3c-0.3,0.2-0.6,0.5-0.8,0.7c-0.6,0.5-1,0.9-1.6,1.1
 c-1.3,0.6-2.2,2-2.2,3.5v2.3h-5.3v-2.2c0-1.5-0.9-2.9-2.2-3.5c-0.6-0.3-1-0.6-1.6-1.2c-0.3-0.2-0.5-0.4-0.8-0.7
 c-1-0.8-2.5-0.9-3.6-0.3l-2.4,1.4l-1.8-3l2.3-1.3c1.2-0.7,1.9-2,1.7-3.4c-0.1-0.6-0.1-1.2-0.1-1.8c0-0.7,0-1.2,0.1-1.8
 c0.2-1.4-0.4-2.8-1.7-3.5l-2.2-1.2l1.7-3l2.4,1.3c1.2,0.7,2.6,0.5,3.6-0.3c0.3-0.2,0.5-0.4,0.8-0.7c0.6-0.6,1.1-0.9,1.6-1.2
 c1.3-0.6,2.2-2,2.2-3.5v-1.9h5.3v1.8c0,1.5,0.9,2.9,2.2,3.5c0.5,0.3,0.9,0.6,1.6,1.1c0.3,0.2,0.6,0.5,0.9,0.7
 c1,0.8,2.4,0.9,3.6,0.3l2.4-1.4l1.8,3l-2.3,1.3C54.6,38.2,53.9,39.6,54.2,41z"
                />
                <path
                  d="M15.3,11.6c-2,0-3.7,1.7-3.7,3.7s1.7,3.7,3.7,3.7s3.7-1.7,3.7-3.7S17.4,11.6,15.3,11.6z"
                />
                <path
                  d="M27,24.6l2.5-4.2c0.3-0.6,0.4-1.3,0.3-2s-0.6-1.2-1.2-1.5L26.8,16c0-0.3,0-0.5,0-0.8c0-0.3,0-0.5,0-0.8l1.8-1
 c1.1-0.6,1.6-2,1.1-3.2L27,5.7c-0.6-1-2-1.5-3.1-1l-2,1.1c-0.3-0.2-0.6-0.5-0.9-0.7l0-1c0-1.9-1.5-3.4-3.4-3.4h-4.5
 c-1.9,0-3.4,1.5-3.4,3.4v1C9.4,5.4,9.1,5.6,8.8,5.9L7.2,5c-1.6-0.9-3-0.2-3.6,0.8L1.1,10c-0.3,0.6-0.4,1.3-0.3,2
 c0.2,0.7,0.6,1.2,1.2,1.5l1.7,1c0,0.2,0,0.5,0,0.8c0,0.2,0,0.5,0,0.7L2,17c-1.1,0.6-1.6,2-1.1,3.2l2.6,4.5c0.6,1.1,2,1.5,3.1,1
 l2-1.1c0.3,0.2,0.6,0.5,1,0.7l0,1.2c0,1.9,1.5,3.4,3.4,3.4h4.5c1.9,0,3.4-1.5,3.4-3.4v-1.3c0.3-0.2,0.6-0.5,0.9-0.7l1.6,0.9
 C24.9,26.3,26.4,25.7,27,24.6z M19.8,20.4c-0.2,0.2-0.4,0.3-0.6,0.5c-0.4,0.4-0.6,0.5-0.9,0.7c-1.2,0.6-1.9,1.7-1.9,3v0.8h-2.2
 v-0.8c0-1.3-0.8-2.5-1.9-3c-0.3-0.1-0.5-0.3-1-0.7c-0.2-0.2-0.4-0.3-0.6-0.5c-0.9-0.8-2.2-0.9-3.3-0.3l-1,0.6L6,19.9l0.9-0.5
 c1.1-0.6,1.7-1.8,1.5-3c0-0.4-0.1-0.8-0.1-1.2c0-0.4,0-0.8,0.1-1.1C8.6,12.9,8,11.6,6.9,11L6,10.5l0.5-0.8l1,0.6
 c1.1,0.6,2.3,0.5,3.3-0.3c0.2-0.2,0.4-0.3,0.5-0.5c0.4-0.4,0.7-0.6,1-0.7c1.2-0.6,1.9-1.7,1.9-3V5.3h2.2v0.5c0,1.3,0.7,2.5,1.9,3
 c0.3,0.1,0.5,0.3,0.9,0.7c0.2,0.2,0.4,0.3,0.6,0.5c0.9,0.8,2.2,0.9,3.3,0.3l1-0.6l0.5,0.8L23.7,11c-1.1,0.6-1.7,1.9-1.5,3.1
 c0.1,0.3,0.1,0.7,0.1,1.1c0,0.4,0,0.7-0.1,1.1c-0.2,1.3,0.4,2.5,1.5,3.1l0.8,0.5l-0.5,0.8l-1-0.6C22,19.5,20.7,19.6,19.8,20.4z"
                />
              </g>
            </svg>
          </div>
          <div class="flex-grow pl-4">
            <h2
              class="font-medium title-font text-2xl text-blue-400 mb-1 tracking-wider"
            >
              PUC - 12th Std
            </h2>
            <p class="leading-relaxed text-gray-300 text-lg">
              Jaimatha Senior Secondary School, Kasaragod, Kerala
            </p>
          </div>
        </div>
        <div class="flex relative">
          <div
            class="flex-shrink-0 w-10 h-10 rounded-full bg-gray-400 inline-flex items-center justify-center text-white relative z-10"
          >
            <!-- Generator: Adobe Illustrator 22.0.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
            <svg
              fill="#1C2033"
              width="30"
              height="30"
              version="1.1"
              id="lni_lni-graduation"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              x="0px"
              y="0px"
              viewBox="0 0 64 64"
              style="enable-background:new 0 0 64 64;"
              xml:space="preserve"
            >
              <path
                d="M61.5,34l-4.2-4.3v-3.8c0.6-0.7,1-1.6,1-2.6c0-1.5-0.8-2.8-2.2-3.4L31.6,8.9c-0.9-0.4-2-0.4-3,0L4,19.8
	c-1.3,0.6-2.2,1.9-2.2,3.4c0,1.5,0.9,2.8,2.2,3.4l8.4,3.8v11.8c0,7.3,5.9,13.2,13.1,13.2h9.1c7.3,0,13.1-5.9,13.1-13.2V30.6l4.8-2.2
	l0.3-0.1v1.6l-4,4.1c-1.1,1.1-1.1,2.8,0,3.9l4.3,4.5c0.5,0.5,1.2,0.8,2,0.8c0,0,0,0,0,0c0.7,0,1.5-0.3,2-0.8l4.3-4.5
	C62.5,36.8,62.5,35.1,61.5,34z M43.2,42.2c0,4.8-3.9,8.7-8.6,8.7h-9.1c-4.8,0-8.6-3.9-8.6-8.7v-9.7l11.9,5.4c0.5,0.2,1,0.3,1.5,0.3
	s1-0.1,1.5-0.3l11.4-5.1V42.2z M30.3,33.5L7.4,23.2l22.7-10l22.6,10.2L30.3,33.5z M55.1,38l-2-2l2-2l2,2L55.1,38z"
              />
            </svg>
          </div>
          <div class="flex-grow pl-4">
            <h2
              class="font-medium title-font text-2xl text-blue-400 mb-1 tracking-wider"
            >
              BE - Computer Science
            </h2>
            <p class="leading-relaxed text-gray-300 text-lg">
              St Joseph Engineering College, Mangaluru
            </p>
          </div>
        </div>
      </div>
      <div class="animation ml-24 mt-0">
        <LottiePlayer
          src="https://assets7.lottiefiles.com/packages/lf20_KWUxUaGUE7.json"
          autoplay={true}
          loop={true}
          controls={false}
          renderer="svg"
          background="transparent"
          height={600}
          width={600}
          {controlsLayout}
        />
      </div>
      <!-- <img class="lg:w-3/5 md:w-1/2 object-cover object-center rounded-lg md:mt-0 mt-12" src="https://dummyimage.com/1200x500" alt="step"> -->
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
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }
</style>
