<script>
  import Step from "./Step.svelte";

  let steps = [
    { name: "Fant-Fash E-commerce Website", icon: "fa-solid fa-cart-shopping" },
    { name: "Toll Collection System", icon: "fa-solid fa-diagram-project" },
    { name: "Everyday Todos", icon: "fa-solid fa-list-check" },
  ];
</script>

<main class="flex flex-col p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi I'm <span class="poppins text-violet-400">Digvijay</span>Adsul
        <br />Full Stack
        <span class="poppins text-violet-400"> Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400">favorite tech</span> includes Python, Django,
        Flask, HTML5, CSS3, JavaScript, ReactJS, Bootstrap, TailwindCSS, MySQL &
        GitHub
      </p>
      <a
        class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins
        relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
        href="https://www.linkedin.com/in/digvijay-adsul"
        target="_blank"
      >
        <div
          class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative z-9">Get in Touch &rarr;</h4>
      </a>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img
        src={"images/profile.jpg"}
        alt="Profile Image"
        class="object-cover z-[2] max-h-[70vh] rounded-3xl"
      />
    </div>
  </section>

  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text-xl md:text-2xl">
        A few of my creative endeavors.
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="poppins text-violet-400">see</span> my work?
      </h3>
    </div>
    <a
      href="https://github.com/Digv06/E-commerce"
      target="_blank"
      class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-12 hover:border-violet-700 duration-200"
    >
      <i class="fa-regular fa-circle-play" />
      <p>Watch the work</p>
    </a>

    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>
          "Fant-Fash" is a responsive website with features such as a tracking
          system, item categorizations and item checkout using <strong
            class="text-violet-400"
            >Django, SQLite, HTML, CSS, JS, and Bootstrap</strong
          >
          and available on GitHub. <br /> Items on the site can be browsed,
          added to the cart, considered, and tracked with one click. <br /> The UI
          has been identified and utilised in around 8-10 projects, with all components
          functioning efficiently.
        </p>
      </Step>

      <Step step={steps[1]}>
        <p>
          Created an Android app with user and admin interface accessibility,
          toll traffic will be decreased by up to 60%, and transaction success
          rate will be 10% higher than currently used one which is build with
          <strong class="text-violet-400">
            Solidity, MetaMask, Web3, HTML, CSS</strong
          >
          To examine the entire money gathered from MetaMask wallet, a web app was
          constructed with the amount kept on Firebase and connected to the smart
          contract written using Remix IDE. <br />
          A research paper has been published on the topic for ref DOI:10.1109/I2CT57861.2023.10126123
        </p>
      </Step>

      <Step step={steps[2]}>
        <p>
          Lorem ipsum dolor sit <strong class="text-violet-400"
            >Tech Languages</strong
          > amet consectetur adipisicing elit. Voluptate consequatur quae quisquam
          voluptas molestiae, accusantium sint repudiandae quam earum velit eos facilis
          impedit excepturi omnis architecto sed blanditiis odit amet unde veniam.
        </p>
      </Step>
    </div>
  </section>

  <section
    id="about"
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-24 relative"
  >
    <div class="">
      <h2>Hello</h2>
    </div>
  </section>
</main>
