<template>
    <div class="sticky top-0 bg-green-500 p-4 flex justify-between items-center">

        <!--   left side -->
        <div class="flex items-center">
            <a href="#" class="inline-block p-2 text-indigo-200 hover:text-indigo-100 mr-2">Home</a>
            <a href="#" class="inline-block p-2 text-indigo-200 hover:text-indigo-100">About</a>
        </div>

        <!--   right side -->
        <div class="hidden md:block">
            <a href="#" class="inline-block p-2 text-indigo-200 hover:text-indigo-100 mr-2">Login</a>
            <a href="#"
               class="inline-block py-2 px-4 text-yellow-700 bg-yellow-400 hover:bg-yellow-300 hover:text-yellow-800 rounded transition ease-in duration-150">Sign
                Up</a>
        </div>

    </div>
</template>

<script>
    export default {
        name : "HeaderComponent",
    }
</script>

<style scoped>

</style>