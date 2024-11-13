<template>
   <div class="relative">
      <img src="/hero_desktop.png" alt="" class="min-h-[550px] object-cover" />
      <div
         class="absolute inset-0 flex flex-col justify-center items-center gap-5 font-bold text-center"
      >
         <h1 class="text-xl md:text-4xl font-bold text-white">
            Discover restaurants and more near you.
         </h1>
         <div
            class="flex justify-between items-center px-2 py-2 bg-white text-gray-500 text-xs rounded-full"
         >
            <div class="flex items-center">
               <button>
                  <svg
                     xmlns="http://www.w3.org/2000/svg"
                     width="24"
                     height="24"
                     viewBox="0 0 24 24"
                     fill="none"
                     stroke="currentColor"
                     stroke-width="2"
                     stroke-linecap="round"
                     stroke-linejoin="round"
                     class="lucide lucide-map-pin"
                  >
                     <path
                        d="M20 10c0 4.993-5.539 10.193-7.399 11.799a1 1 0 0 1-1.202 0C9.539 20.193 4 14.993 4 10a8 8 0 0 1 16 0"
                     />
                     <circle cx="12" cy="10" r="3" />
                  </svg>
               </button>
               <input
                  type="text"
                  placeholder="Enter your address"
                  class="px-4 md:py-2 rounded-full md:w-64 outline-none"
               />
            </div>

            <button>
               <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
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
         <div
            class="flex items-center text-blak bg-white text-xs rounded-full px-2 py-1 gap-2"
         >
            <button class="rounded-full">
               <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="20"
                  height="20"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="lucide lucide-user"
               >
                  <path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2" />
                  <circle cx="12" cy="7" r="4" />
               </svg>
            </button>
            <p>Sign in for saved address</p>
         </div>
      </div>
   </div>
</template>
