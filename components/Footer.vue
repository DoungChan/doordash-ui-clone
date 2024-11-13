<template>
   <div class="bg-black px-8 md:px-32 py-14 text-white">
      <div
         class="flex flex-col md:justify-center md:items-center gap-4 md:gap-12 w-fit m-auto md:m-0"
      >
         <div class="flex flex-col w-full">
            <h1 class="text-lg font-bold mb-4">Popular Categories</h1>
            <div class="flex flex-col sm:flex-row flex-wrap max-w-full">
               <p
                  v-for="i in categories"
                  :key="i"
                  class="w-full sm:w-1/2 md:w-1/4 mt-2 text-xs text-nowrap"
               >
                  {{ i }}
               </p>
            </div>
         </div>
         <div class="w-full">
            <div
               class="flex flex-col justify-start items-start md:flex-row md:flex-wrap w-full md:w-1/2"
            >
               <div class="flex flex-col flex-1 mb-4 md:mb-0">
                  <h1 class="text-lg font-bold mb-4">Get to Know Us</h1>
                  <div class="flex flex-col">
                     <div
                        v-for="i in getToKnowUs"
                        :key="i"
                        class="w-full md:w-1/4 mt-2"
                     >
                        <p class="text-xs text-nowrap">{{ i }}</p>
                     </div>
                  </div>
               </div>
               <div class="flex flex-col flex-1 mb-4 md:mb-0">
                  <h1 class="text-lg font-bold mb-4">Let Us Help You</h1>
                  <div class="flex flex-col">
                     <div
                        v-for="i in letUsHelpYou"
                        :key="i"
                        class="w-full md:w-1/4 mt-2"
                     >
                        <p class="text-xs text-nowrap">{{ i }}</p>
                     </div>
                  </div>
               </div>
               <div class="flex flex-col flex-1">
                  <h1 class="text-lg font-bold mb-4">Doing Business</h1>
                  <div class="flex flex-col">
                     <div
                        v-for="i in doingBusiness"
                        :key="i"
                        class="w-full md:w-1/4 mt-2"
                     >
                        <p class="text-xs text-nowrap">{{ i }}</p>
                     </div>
                  </div>
               </div>
            </div>
         </div>
      </div>
   </div>
</template>

<script setup>
   const categories = [
      "Alcohol Australia",
      "Alcohol Delivery Australia",
      "Back To School Delivery",
      "Beauty Stores",
      "Beauty Supply",
      "Catering Near Me",
      "Chips Ahoy Big Cookie",
      "Convenience Stores Canada",
      "Dashmart Near Me",
      "Deck The Doorstep",
      "Diageo Holiday",
      "Drugstores Canada",
      "Flower Delivery",
      "Grocery Delivery Canada",
      "Haleon Well Within Reach",
      "Halloween",
      "Hsa Bank",
      "Hsa Fsa Store",
      "Large Group Orders",
      "Medicine Delivery",
      "Mothers Day",
      "Pet Store Near Me",
      "Retail Stores Near Me",
      "Seasonal Holidays",
      "Snap Ebt",
      "Valentines Day",
      "Winter Holidays",
   ];
   const getToKnowUs = [
      "About Us",
      "Careers",
      "Investors",
      "Company Blog",
      "Engineering Blog",
      "Merchant Blog",
      "Gift Cards",
      "Package Pickup",
      "Promotions",
      "Dasher Central",
      "LinkedIn",
      "Glassdoor",
      "Accessibility",
      "Newsroom",
   ];

   const letUsHelpYou = ["Account Details", "Order History", "Help"];

   const doingBusiness = [
      "Become a Dasher",
      "List Your Business",
      "Get Dashers for Deliveries",
      "Get DoorDash for Business",
   ];
</script>
