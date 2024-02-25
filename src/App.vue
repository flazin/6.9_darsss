<script setup>
import { ref } from "vue";

let open = ref(false);
</script>

<template>
  <header class="bg-indigo-500">
    <nav
      class="container relative flex items-center justify-between px-6 py-8 mx-auto text-white"
    >
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
        class="absolute inset-x-0 z-30 w-full px-6 py-8 mt-4 space-y-6 transition-all duration-300 ease-in-out bg-indigo-600 top-16 md:mt-0 md:p-0 md:top-0 md:relative md:bg-transparent md:w-auto md:opacity-100 md:translate-x-0 md:space-y-0 md:-mx-6 md:flex md:items-center"
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
          <h1 class="title">
            Hi , I’m Charles, <br /><br /><br /><br /><br />
            Front-end Developer
          </h1>

          <p class="desc">
            I design and develop experiences that make people’s lives
            <br /><br /><br /><br /><br /><br /><br />
            simpler through Web and Mobile apps.I work with FIgma ,
            <br /><br /><br /><br /><br /><br /><br />
            HTML5, CSS3, JavaScript, React, ReactNative and Flutter.
          </p>

          <button class="here">HERE ME</button>
          <button class="hare">SEE MY PROJECTS</button>
        </div>
      </div>
    </section>
  </main>
</template>
