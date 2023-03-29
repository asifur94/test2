<template>
 

  


    <section  class="w-fit   mx-auto grid grid-cols-1 lg:grid-cols-3 md:grid-cols-2 justify-items-center justify-center gap-y-20 gap-x-14 mt-10 mb-5">
                      
      <!--   ✅ Product card 1 - Starts Here 👇 -->
      <div v-for="courses in course" class="w-52 bg-white shadow-md flex justify-end rounded-xl duration-500 hover:scale-105 hover:shadow-xl">
        <div >
          <NuxtLink  v-on:click="count += 1">
          <img src="{{courses.image}}" alt="" class="h-52 w-52 object-cover rounded-t-xl">
          
          </NuxtLink>
          <div class="px-4 py-3 w-52">
            
            <p class="text-lg font-bold text-black truncate block capitalize">{{ courses.name }}</p>
            <span class="text-gray-400 mr-3 uppercase text-xs">{{  courses.description  }} </span>
            <div class="flex items-center">
              <p class="text-lg font-semibold text-red-700 cursor-auto my-3">{{courses.price}}</p>
              <del>
                
              </del>
              <div class="ml-auto">
  
  
              </div>
            </div>
          </div>
        </div>
      </div>
     
      </section>
  
     
      
      
  </template>
  
  <script>
  
export default {
  props: ['course'],


    
};
  
    

  
  </script>
  