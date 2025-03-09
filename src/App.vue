<template>
    <div class="text-gray-900 pt-1 ">
        <hr>
        <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-3 ">
            <div class="col-span-1 md:flex md:justify-end">
                <nav class="md:text-right ">
                    <div class="flex justify-between items-center py-3">
                        <h1
                            class="text-slate-500 font-bold uppercase text-sm md:text-lg lg:text-lg hover:text-slate-900 ">
                            <a href="/">Kent Main Dishes</a>
                        </h1>
                        <div class="cursor-pointer fixed right-0" @click="togglebtn = !togglebtn">
                            <span v-if="!togglebtn">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-8 block md:hidden">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 5.25h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5m-16.5 4.5h16.5" />
                              </svg>
                            </span>
                            <span v-else>
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-8 block md:hidden">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                                </svg>
                            </span>
                            
                        </div>
                    </div>
                    

                    <ul class="text-sky-700 py-6  hidden md:block">
                        <li>
                            <a href="#" class="flex | gap-3 | md:justify-end border-r-4 border-white hover:border-customcolor duration-200 ease pr-2">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="size-6 w-5 md:mr-3">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="m2.25 12 8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
                                </svg>
                                <span>Home</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="flex | gap-3 | md:justify-end border-r-4 border-white hover:border-customcolor duration-200 ease pr-2">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="size-6 w-5 md:mr-3">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M9.879 7.519c1.171-1.025 3.071-1.025 4.242 0 1.172 1.025 1.172 2.687 0 3.712-.203.179-.43.326-.67.442-.745.361-1.45.999-1.45 1.827v.75M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Zm-9 5.25h.008v.008H12v-.008Z" />
                                </svg>
                                <span>About</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="flex | gap-3 | md:justify-end border-r-4 border-white hover:border-customcolor duration-200 ease pr-2">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="size-6 w-5">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 0 0 2.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 0 1-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 0 0-1.091-.852H4.5A2.25 2.25 0 0 0 2.25 4.5v2.25Z" />
                                </svg>
                                <span>Contact</span>
                            </a>
                        </li>
                    </ul>


                </nav>
                
            </div>

            <main class="bg-gray-100 | col-span-2 | px-16">

                <div class="flex justify-center mx-auto" v-if="togglebtn">
                    <Navigation/>
                </div>
                
                <div class="text-blue-700 | flex justify-center | gap-1.5 md:justify-end lg:justify-end">
                    <a href="#"
                        class="text-customcolor rounded-full py-1 px-3 mt-2 cursor-pointer md:border-2 hover:bg-customcolor hover:text-white font-Poppins duration-200 ease-in">Log
                        in</a>
                    <a href="#"
                        class="text-customcolor rounded-full py-1 px-3 mt-2 cursor-pointer md:border-2 hover:bg-customcolor hover:text-white font-Poppins duration-200 ease-in">Sign
                        up</a>
                </div>

                <header class="pb-6">
                    <h2 class="text-4xl font-bold text-zinc-700 | font-Poppins">Recipes</h2>
                    <h3 class="text-violet-500 font-semibold">For fat asses!</h3>
                </header>

                <div class="py-3">
                    <h4 class="text-2xl font-semibold text-stone-900 mb-3 border-b-2 border-blue-500">Latest Recipes
                    </h4>
                    <div class="grid grid-cols-1 gap-10  md:grid-cols-3 lg:grid-cols-3">
                        <!-- cards go here -->
                        <div class="card hover:drop-shadow-lg duration-150 ease-in">
                            <img src="/src/assets/stew.jpg" alt="stew" class="w-full | h-60 | lg:h-32 | object-cover">
                            <div class="p-2">
                                <span class="font-Poppins | font-bold">5 Bean Chili Stew</span>
                                <span class="font-Poppins | block | text-gray-500">Recipe by Mario</span>
                            </div>
                            <div class="badge | flex | items-center | gap-1">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="size-6 w-5">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M12 6v6h4.5m4.5 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                                </svg>
                                <span class=""> 30 mins</span>
                            </div>
                        </div>
                        <div class="card hover:drop-shadow-lg duration-150 ease-in">
                            <img src="/src/assets/ramen.jpg" alt="ramen" class="w-full | h-60 | lg:h-32 | object-cover">
                            <div class="p-2">
                                <span class="font-Poppins | font-bold">Ichiraku Ramen</span>
                                <span class="font-Poppins | block | text-gray-500">Recipe by Teuchi Ichiraku</span>
                            </div>
                            <div class="badge | flex | items-center | gap-1">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="size-6 w-5">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M12 6v6h4.5m4.5 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                                </svg>
                                <span class=""> 1 hr</span>
                            </div>
                        </div>
                        <div class="card hover:drop-shadow-lg duration-150 ease-in">
                            <img src="/src/assets/curry.jpg" alt="curry" class="w-full | h-60 | lg:h-32 | object-cover">
                            <div class="p-2">
                                <span class="font-Poppins | font-bold">Curry</span>
                                <span class="font-Poppins | block | text-gray-500">Recipe by Hannah Glasse</span>
                            </div>
                            <div class="badge | flex | items-center | gap-1">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="1.5" stroke="currentColor" class="size-6 w-5">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M12 6v6h4.5m4.5 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                                </svg>
                                <span class=""> 50 mins</span>
                            </div>
                        </div>
                    </div>
                </div>
                <h4 class="pt-12 border-b-2 border-blue-500">Most Popular</h4>
                <div>
                    <!-- cards go here -->
                </div>
                <div class="flex | mt-2 | cursor-pointer | justify-center | items-center">
                    <div class="buttons hover:shadow-inner">Load more</div>
                </div>
            </main>
        </div>
    </div>
</template>
<script>
import { ref } from "vue";
import Navigation from './components/Navigation.vue';
    export default {
        components: {
            Navigation,
        },
        name: 'App',
        setup(){
            
            const togglebtn = ref(false);
           

            return {
                togglebtn,
            }
        }
       
    }
</script>


<style scoped>

</style>