<template>
  <div class="flex flex-wrap">
    <div class="rounded w-full bg-orange-300 p-4">
      Banner
      <button class="block rounded-md shadow-md px-4 py-2 bg-orange-600">CTA</button>
    </div>
    <div class="rounded w-full bg-orange-500 p-4 flex flex-col md:flex-row">
      <div class="w-full p-4 bg-">
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Suscipit, rem officia blanditiis quaerat ea ab accusantium, delectus velit cupiditate maiores, quia ex nobis dolore quas ullam ut rerum vero in.</p>
      </div>
      <div class="w-full bg-green-600 rounded-md p-4">
        Tools/Languages 
      </div>
    </div>
    <div class="rounded w-full bg-yellow-500 p-4">
  <div class="experiences grid grid-cols-1 md:grid-cols-2 gap-2 p-4">
    <!-- Experiences -->
    <div class="flex flex-row flex-nowrap overflow-x-auto md:flex-col gap-4 justify-center items-center w-full">
      <div class="bg-slate-400 rounded-md shadow-sm py-4 px-2 h-15 flex items-center justify-center md:w-full w-[100px]">Freelance</div>
      <div class="bg-slate-400 rounded-md shadow-sm py-4 px-2 h-15 flex items-center justify-center md:w-full w-[100px]">LawAdvisor</div>
      <div class="bg-slate-400 rounded-md shadow-sm py-4 px-2 h-15 flex items-center justify-center md:w-full w-[100px]">Yondu</div>
      <div class="bg-slate-400 rounded-md shadow-sm py-4 px-2 h-15 flex items-center justify-center md:w-full w-[100px]">Sparksoft</div>
      <div class="bg-slate-400 rounded-md shadow-sm py-4 px-2 h-15 flex items-center justify-center md:w-full w-[100px]">Straightarrow</div>
      <div class="bg-slate-400 rounded-md shadow-sm py-4 px-2 h-15 flex items-center justify-center md:w-full w-[100px] ">One Click Travel</div>
    </div>

    <div class="bg-black text-white">
      <h3>Job Position</h3>
      <small>Dates</small>
      <ul class="experience-list list-disc ml-5">
        <li>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam debitis delectus, libero quod perspiciatis rem dolorem. Ipsum placeat, repellendus, culpa beatae, assumenda laborum rerum iure odit asperiores voluptate reprehenderit molestiae!
        </li>
        <li>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam debitis delectus, libero quod perspiciatis rem dolorem. Ipsum placeat, repellendus, culpa beatae, assumenda laborum rerum iure odit asperiores voluptate reprehenderit molestiae!
        </li>
        <li>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam debitis delectus, libero quod perspiciatis rem dolorem. Ipsum placeat, repellendus, culpa beatae, assumenda laborum rerum iure odit asperiores voluptate reprehenderit molestiae!
        </li>
        <li>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam debitis delectus, libero quod perspiciatis rem dolorem. Ipsum placeat, repellendus, culpa beatae, assumenda laborum rerum iure odit asperiores voluptate reprehenderit molestiae!
        </li>
      </ul>
    </div>
  </div>
</div>
    <div class="rounded w-full bg-green-500 p-4">
      <div class="flex flex-wrap gap-4">
        <div
        v-for="(item, index) in items"
        :key="index"
        class="w-full rounded-md p-3"
        :class="{
          'text-left bg-blue-400': isOdd(index),
          'text-right bg-blue-500': !isOdd(index),
        }"
      >
        {{ item }}
      </div>
      </div>
    </div>
    <div class="rounded w-full bg-red-500 p-4 flex justify-center items-center">
      <p>Get in touch</p>
      <button>
        Let's talk
      </button>
      </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
const items = ref([1, 2, 3, 4]);
const isOdd = (index) => index % 2 === 0;
</script>