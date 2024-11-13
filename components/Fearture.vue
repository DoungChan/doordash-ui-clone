<template>
   <div class="flex flex-col justify-center items-center gap-2 w-1/2 md:w-1/6">
      <img :src="img" alt="" />
      <h1 class="text-xl md:text-3xl font-bold text-center">{{ title }}</h1>
      <p class="text-center">
         {{ description }}
      </p>
      <div
         class="flex justify-center items-center text-orange-600 cursor-pointer gap-2"
      >
         <p>{{ link }}</p>
         <button>
            <svg
               width="20"
               height="20"
               viewBox="0 0 24 24"
               fill="none"
               stroke="currentColor"
               stroke-width="2"
               stroke-linecap="round"
               stroke-linejoin="round"
               class="lucide lucide-arrow-right"
            >
               <path d="M5 12h14" />
               <path d="m12 5 7 7-7 7" />
            </svg>
         </button>
      </div>
   </div>
</template>
<script>
   export default {
      name: "Feature",
      props: {
         img: String,
         title: String,
         description: String,
         link: String,
      },
   };
</script>
