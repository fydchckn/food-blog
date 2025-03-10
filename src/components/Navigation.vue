<template>
    <div class="fixed inset-0 bg-gradient-to-b from-black/0 to-black/80 opacity-100 z-1"></div>
    
    <div  class="w-[80%] bg-black  text-center fixed md:hidden  font-Poppins text-lg leading-10 p-5 l rounded-2xl backdrop-blur-xs z-2">
        <div>
            <nav>
                <ul class="text-white ">
                    <li class="hover:text-customcolor duration-100 ease"><a href="#">Home</a></li>
                    <li class="hover:text-customcolor duration-100 ease"><a href="#">About</a></li>
                    <li class="hover:text-customcolor duration-100 ease"><a href="#">Contact</a></li>
                </ul>
            </nav>
        </div>
    </div>
                        
</template>

<script>
export default {
    name: "Navigation",
}
</script>

<style>

</style>