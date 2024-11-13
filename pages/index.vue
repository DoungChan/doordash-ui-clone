<template>
   <div>
      <AppHeader />
      <!-- Herosection -->
      <HeroDesktop />
      <!-- Fearturesectior -->
      <div
         class="flex flex-col md:flex-row justify-evenly items-center gap-4 py-32"
      >
         <Fearture
            v-for="(item, index) in fearture"
            :key="index"
            :img="item.img"
            :title="item.title"
            :description="item.text"
            :link="item.link"
         />
      </div>
      <!-- CustomCTAWrapper -->
      <div class="w-full">
         <div
            class="flex flex-col md:flex-row-reverse justify-center items-center gap-4 md:gap-16 px-4 lg:px-32 -mb-64 md:-mb-10"
         >
            <div class="w-full">
               <img
                  src="https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/download_the_app_desktop.png"
                  alt=""
                  class="w-full h-[180px] md:h-[500px] object-cover"
               />
            </div>

            <div class="flex flex-col gap-4 item-center">
               <div class="flex flex-col gap-4">
                  <h1 class="text-xl md:text-4xl font-bold">
                     Everything you crave, delivered.
                  </h1>
                  <h6 class="font-bold text-sm">
                     Your favorite local restaurants
                  </h6>
                  <p class="text-sm">
                     Get a slice of pizza or the whole pie delivered, or pick up
                     house lo mein from the Chinese takeout spot you've been
                     meaning to try.
                  </p>
               </div>

               <button
                  class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit"
               >
                  Find restaurants
               </button>
            </div>
         </div>
      </div>
      <div class="bg-[#fef1ee] py-28">
         <div
            class="flex flex-col md:flex-row justify-center items-center gap-4 md:gap-16 px-4 mt-64 md:mt-0 lg:px-32"
         >
            <div class="w-full">
               <img
                  src="https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/dashpass_desktop.png"
                  alt=""
                  class="w-full h-[180px] md:h-[500px] object-cover"
               />
            </div>

            <div class="flex flex-col gap-4 text-left">
               <div class="flex flex-col gap-4">
                  <h1 class="text-xl md:text-4xl font-bold">
                     DashPass is delivery for less
                  </h1>

                  <p class="text-sm">
                     Members get a $0 delivery fee on DashPass orders, 5% back
                     on pickup orders, and so much more. Plus, it's free for 30
                     days.
                  </p>
               </div>

               <button
                  class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit"
               >
                  Get DashPass
               </button>
            </div>
         </div>
      </div>
      <!-- Gocery -->
      <div
         class="relative h-[350px] md:h-[600px] bg-[url('/grocery_desktop.avif')] bg-cover bg-center"
      >
         <div
            class="w-full h-full relative z-10 top-0 left-0 flex text-center justify-center items-center bg-black bg-opacity-60"
         >
            <div
               class="flex flex-col gap-4 justify-center items-center max-w-[550px] mt-auto mb-auto text-white"
            >
               <div class="flex flex-col gap-4">
                  <h1 class="text-xl md:text-4xl font-bold">
                     Get grocery and convenience store essentials
                  </h1>
                  <h6 class="font-bold text-sm md:text-lg">
                     Grocery delivery, exactly how you want it.
                  </h6>
                  <p class="text-xs md:text-sm">
                     Shop from home and fill your cart with fresh produce,
                     frozen entrees, deli delights and more.
                  </p>
               </div>
               <button
                  class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit"
               >
                  Shop Groceries
               </button>
            </div>
         </div>
      </div>
      <!-- shop -->
      <div class="w-full">
         <div
            class="flex flex-col md:flex-row-reverse justify-center items-center gap-4 md:gap-16 px-4 lg:px-32 md:-mb-10 pt-4 md:pt-12"
         >
            <div class="w-full">
               <img
                  src="/convenience_desktop.avif"
                  alt=""
                  class="w-full h-[180px] md:h-[500px] object-cover"
               />
            </div>

            <div class="flex flex-col gap-4 item-center">
               <div class="flex flex-col gap-4">
                  <h1 class="text-xl md:text-4xl font-bold">
                     Convenience stores at your doorstep
                  </h1>

                  <p class="text-sm">
                     Stock up on snacks, household essentials, candy, or
                     vitamins — all delivered in under an hour.
                  </p>
               </div>

               <button
                  class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit"
               >
                  Shop Now
               </button>
            </div>
         </div>
      </div>
      <!-- Gift -->
      <div
         class="w-full flex flex-col p-12 md:pt-20 bg-[#fef1ee] items-start justify-start gap-12 mt-2 md:mt-0 overflow-hidden"
      >
         <h1 class="text-xl md:text-3xl font-bold m-auto md:w-1/3 text-center">
            Helping you with to-dos and gifting
         </h1>
         <div
            class="flex max-w-[100%] md:flex-wrap md:max-w-[1280px] overflow-x-auto scrollbar-hide"
         >
            <div
               v-for="i in gifting"
               :key="i"
               class="w-screen md:w-1/2 p-4 flex-shrink-0"
            >
               <div class="flex flex-col items-center">
                  <img
                     :src="i.img"
                     alt=""
                     class="inset-0 h-[180px] md:h-full w-full object-cover"
                  />
                  <div
                     class="flex flex-col gap-4 m-auto px-2 text-center mt-4 justify-center items-center"
                  >
                     <h1 class="text-xl md:text-4xl font-bold">
                        {{ i.title }}
                     </h1>
                     <p class="text-xs md:text-sm">
                        {{ i.text }}
                     </p>
                     <button
                        class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit mt-4"
                     >
                        {{ i.link }}
                     </button>
                  </div>
               </div>
            </div>
         </div>
      </div>
      <!-- opportunity -->
      <div class="w-full">
         <h1
            class="text-xl md:text-3xl font-bold m-auto md:w-1/3 text-center py-12"
         >
            Helping you with to-dos and gifting
         </h1>
         <div
            class="flex flex-col md:flex-row-reverse justify-center items-center gap-4 md:gap-16 px-4 lg:px-32 -mb-64 md:-mb-10"
         >
            <div class="w-full">
               <img
                  src="https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/become_a_dasher_desktop.png"
                  alt=""
                  class="w-full h-[180px] md:h-[500px] object-cover"
               />
            </div>

            <div class="flex flex-col gap-4 item-center">
               <div class="flex flex-col gap-4">
                  <h1 class="text-xl md:text-4xl font-bold">
                     Everything you crave, delivered.
                  </h1>
                  <h6 class="font-bold text-sm">
                     Your favorite local restaurants
                  </h6>
                  <p class="text-sm">
                     Get a slice of pizza or the whole pie delivered, or pick up
                     house lo mein from the Chinese takeout spot you've been
                     meaning to try.
                  </p>
               </div>

               <button
                  class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit"
               >
                  Find restaurants
               </button>
            </div>
         </div>
      </div>
      <div class="bg-[#fef1ee] py-28">
         <div
            class="flex flex-col md:flex-row justify-center items-center gap-4 md:gap-16 px-4 mt-64 md:mt-0 lg:px-32"
         >
            <div class="w-full">
               <img
                  src="https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/work_with_doordash_desktop.png"
                  alt=""
                  class="w-full h-[180px] md:h-[500px] object-cover"
               />
            </div>

            <div class="flex flex-col gap-4 text-left">
               <div class="flex flex-col gap-4">
                  <h1 class="text-xl md:text-4xl font-bold">
                     Everything you crave, delivered.
                  </h1>
                  <h6 class="font-bold text-sm">
                     Your favorite local restaurants
                  </h6>
                  <p class="text-sm">
                     Get a slice of pizza or the whole pie delivered, or pick up
                     house lo mein from the Chinese takeout spot you've been
                     meaning to try.
                  </p>
               </div>

               <button
                  class="bg-[#eb1700] text-white text-sm font-bold px-4 py-2 rounded-full w-fit"
               >
                  Find restaurants
               </button>
            </div>
         </div>
      </div>
      <!-- Footer -->
      <Footer />
   </div>
</template>
<script setup>
   const fearture = [
      {
         img: "/ScootScoot.svg",
         title: "Become a Dasher",
         text: "As a delivery driver, make money and work on your schedule. Sign up in minutes.",
         link: "Start earning",
      },
      {
         img: "/Storefront.svg",
         title: "Become a Merchantr",
         text: "As a delivery driver, make money and work on your schedule. Sign up in minutes.",
         link: "Start earning",
      },
      {
         img: "/iphone.svg",
         title: "Get the best DoorDash experience",
         text: "As a delivery driver, make money and work on your schedule. Sign up in minutes.",
         link: "Start earning",
      },
   ];

   const gifting = [
      {
         img: "https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/package_pickup_desktop.png",
         title: "Return packages from home",
         text: "Request a package pickup with just a few taps and get your returns dropped off at carriers like UPS, FedEx, and USPS.",
         link: "Try Package Pickup",
      },
      {
         img: "/flowers_desktop.avif",
         title: "Flowers for any occasion",
         text: "Shop hand-picked and thoughtfully-arranged blooms from florists near you.",
         link: "Send flowers",
      },
      {
         img: "https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/alcohol_desktop.png",
         title: "Restock the minibar",
         text: "Hosting a get-together or need or need a special cocktail ingredient? Get liquor, beer, mixers, champagne and wine delivered fast.*",
         link: "Shop alcohol",
      },
      {
         img: "https://img.cdn4dd.com/cdn-cgi/image/fit=cover,format=auto,quality=60/https://cdn.doordash.com/managed/consumer/seo/home/landing_cta/pet_supplies_desktop.png",
         title: "What your pets need, and want",
         text: "Finally, something cat people and dog people agree on — pet supplies delivery. Shop pet food, chew toys, and even costumes.",
         link: "Get pet supplies",
      },
   ];
</script>
