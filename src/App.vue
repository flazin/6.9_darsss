<script setup>
import { ref } from "vue";

let open = ref(false);
</script>

<template class="body">
  <header class="bg-indigo-500">
    <nav
      class="container relative flex items-center justify-between px-6 py-8 mx-auto text-white"
    >
      <a href="#">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="w-8 h-8 md:w-10 md:h-10"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1 1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-6z"
          />
        </svg>
      </a>

      <button @click="open = !open" class="md:hidden">
        <span v-show="!open">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-6 h-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M4 6h16M4 12h16m-7 6h7"
            />
          </svg>
        </span>

        <span v-show="open">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5"
            viewBox="0 0 20 20"
            fill="currentColor"
          >
            <path
              fill-rule="evenodd"
              d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
              clip-rule="evenodd"
            />
          </svg>
        </span>
      </button>

      <div
        :class="[
          open ? 'translate-x-0 opacity-100 ' : 'opacity-0 -translate-x-full',
        ]"
      >
        <a
          href="#"
          class="block text-white transition-colors duration-300 md:px-6 hover:text-indigo-300"
          >Home
        </a>
        <a
          href="#"
          class="block text-white transition-colors duration-300 md:px-6 hover:text-indigo-300"
        >
          About
        </a>
        <a
          href="#"
          class="block text-white transition-colors duration-300 md:px-6 hover:text-indigo-300"
        >
          Portfolio
        </a>
        <a
          href="#"
          class="block text-white transition-colors duration-300 md:px-6 hover:text-indigo-300"
        >
          Blogs
        </a>
        <a
          href="#"
          class="block text-white transition-colors duration-300 md:px-6 hover:text-indigo-300"
        >
          Contact
        </a>
      </div>
    </nav>
  </header>

  <main>
    <section>
      <div
        class="relative grid w-full bg-indigo-500 h-96 lg:h-[32rem] place-items-center"
      >
        <div class="flex flex-col items-center mx-auto text-center">
          <h1 class="text-2xl font-semibold text-white uppercase md:text-3xl">
            Hi , I’m Charles, Front-end Developer
          </h1>

          <p class="mt-6 text-lg leading-5 text-white">
            I design and develop experiences that make people’s lives simpler
            through Web and Mobile apps.I work with FIgma , HTML5, CSS3,
            JavaScript, React, ReactNative and Flutter.
          </p>

          <button class="here">HERE ME</button>
          <button class="hare">SEE MY PROJECTS</button>
          <a href="#about" class="mt-8 cursor-pointer animate-bounce"> </a>
        </div>
      </div>

      <svg
        class="fill-indigo-500"
        viewBox="0 0 1440 57"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path d="M1440 0H0V57C720 0 1440 57 1440 57V0Z" />
      </svg>
    </section>

    <section class="container px-6 py-8 mx-auto lg:py-16" id="about">
      <div class="lg:flex lg:items-center lg:-mx-4">
        <div class="lg:w-1/2 lg:px-4">
          <h3 class="text-xl font-medium text-gray-800 md:text-2xl lg:text-3xl">
            We create awesome prototypes, plugins, and templates.
          </h3>

          <p class="mt-6 text-gray-500">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic
            laboriosam provident voluptatum id magni iste nobis corrupti,
            delectus quis repellat, debitis error quod explicabo molestiae rerum
            totam ab sunt excepturi?
          </p>

          <button class="flex items-center mt-8 -mx-2 text-indigo-500">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="w-8 h-8 mx-1"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"
              />
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
              />
            </svg>
            <p class="mx-1 font-semibold">PLAY VIDEO</p>
          </button>
        </div>

        <div class="mt-8 lg:w-1/2 lg:px-4 lg:mt-0">
          <img
            class="object-cover w-full rounded-xl h-96"
            src="https://images.unsplash.com/photo-1516131206008-dd041a9764fd?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80"
            alt="Video thumbnail"
          />
        </div>
      </div>
    </section>
  </main>
</template>
