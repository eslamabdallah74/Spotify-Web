<template>
    <!-- component -->
<!-- Header -->
<header>
    <!-- navbar and menu -->
    <nav class="shadow">
  
    <div class="container flex items-center justify-between px-10 py-6 mx-auto">
  
      <div>
        <h1 class="text-2xl font-bold text-transparent bg-gradient-to-tr from-indigo-600 to-green-600 bg-clip-text hover:cursor-pointer">Adsla</h1>
      </div>
  
      <div>
        
        <div class="hover:cursor-pointer sm:hidden">
          <spnan class="block w-8 h-1 mb-1 rounded-full bg-gradient-to-tr from-indigo-600 to-green-600"></spnan>
          <spnan class="block w-8 h-1 mb-1 rounded-full bg-gradient-to-tr from-indigo-600 to-green-600"></spnan>
          <spnan class="block w-8 h-1 mb-1 rounded-full bg-gradient-to-tr from-indigo-600 to-green-600"></spnan>
        </div>
        <div class="flex items-center">
  
          <ul class="items-center hidden space-x-4 sm:flex">
            <li><a href="#" class="text-gray-700 hover:text-indigo-600 text-md ">Home</a></li>
            <li><a href="#" class="text-gray-700 hover:text-indigo-600 text-md ">About</a></li>
            <li><a href="#" class="text-gray-700 hover:text-indigo-600 text-md ">Services</a></li>
            <li><a href="#" class="text-gray-700 hover:text-indigo-600 text-md ">Products</a></li>
            <li><a href="#" class="text-gray-700 hover:text-indigo-600 text-md ">Contact</a></li>
          </ul>
  
          <div class="items-center hidden ml-8 space-x-4 md:flex lg:ml-12">
            <!-- <h1  class="py-2 text-text-gray-600 hover:cursor-pointer hover:text-indigo-600"> <a href="https://www.spotify.com/logout/"> logout </a> </h1> -->
            <h1 class="px-4 py-2 text-white rounded text-text-gray-600 hover:cursor-pointer bg-gradient-to-tr from-indigo-600 to-green-600 hover:shadow-lg">Login</h1>
          </div>
        </div>
      </div>
    </div>
    </nav>
  </header>
  <main>
    <!-- section hero -->
    <section>
      <div class="min-h-full grid-cols-5 grid-rows-2 px-4 py-6 space-y-6 bg-gray-100 sm:grid lg:min-h-screen sm:space-y-0 sm:gap-4">
  
      <div class="col-span-4 rounded-md bg-gradient-to-tr from-indigo-800 to-indigo-500">
        <!-- Slot -->
        <slot />
        
      </div>
      <div class="col-span-1 h-96 ">
        <div class="flex items-center justify-around px-4 py-3 bg-white rounded-lg ">
     <input type="text" placeholder="seach" class="w-full p-2 pl-2 mr-2 bg-gray-100 rounded-md outline-none ring-indigo-700">
    <span><svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor ">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
  </svg></span>
        </div>
        <div class="bg-white rounded-md">
  
        <h1 class="py-2 my-4 text-xl text-center text-gray-600 bg-white border-b-2 rounded-md cursor-pointer">Service</h1>
        <div class="text-center list-none bg-white rounded-md ">
          <li class="py-3 border-b-2"><a href="#" class="list-none hover:text-indigo-600">Products</a></li>
          <li class="py-3 border-b-2"><a href="#" class="list-none hover:text-indigo-600">Models</a></li>
          <li class="py-3 border-b-2"><a href="#" class="list-none hover:text-indigo-600">Pricing</a></li>
          <li class="py-3 border-b-2"><a href="#" class="list-none hover:text-indigo-600">Hire</a></li>
          <li class="py-3 "><a href="#" class="list-none border-b-2 hover:text-indigo-600">Business</a></li>
        </div>
        </div>
      </div>
      </div>
  
    </section>
  
  </main>
</template>