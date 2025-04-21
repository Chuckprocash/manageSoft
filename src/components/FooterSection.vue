<script setup>
    const array = ['facebook.svg', 'pinterest.svg', 'tumblr.svg', 'instagram.svg', 'linkedin.svg'];
</script>
<template>
    <footer class="bg-gray-900">
        <div class="container mx-auto flex flex-col-reverse justify-between px-6 py-10 space-y-8 md:space-y-0 md:flex-row">
            <div class="md:hidden text-white text-center mx-auto my6">
                Copyright &copy; 2023 manage. All rights reserved.
            </div>
            <div class="flex flex-col-reverse items-center justify-between space-y-12 md:space-y-0 md:items-start md:flex-col">
                <div class="flex mb-4 -ml-2">
                    <img src="../assets/lion.svg" class="h-10" alt="logo" />
                    <h4 class="text-3xl font-semibold text-white -ml-4">manage</h4>
                </div>
                <div class="flex justify-center space-x-3">
                    <a href="#" v-for="(item, i) in array" :key="i">
                        <img :src="`/images/${item}`" alt="social" class="h-5" />
                    </a>
                </div>
            </div>
            
            <div class="flex justify-around space-x-12 lg:space-x-32">
                <div class="flex flex-col space-y-3 text-white">
                    <a href="#" class="hover:text-orange-700">Home</a>
                    <a href="#" class="hover:text-orange-700">Pricing</a>
                    <a href="#" class="hover:text-orange-700">Products</a>
                    <a href="#" class="hover:text-orange-700">About</a>
                </div>
                <div class="flex flex-col space-y-3 text-white">
                    <a href="#" class="hover:text-orange-700">Contact</a>
                    <a href="#" class="hover:text-orange-700">Community</a>
                    <a href="#" class="hover:text-orange-700">Privacy Policy</a>
                </div>
            </div>
            <div class="flex flex-col justify-between md:w-1/3">
                <form>
                    <div class="flex space-x-3 mb-6">
                        <input type="text" class="flex-1 px-4 bg-white rounded-full focus:outline-none" 
                        placeholder="Update in your inbox" />
                        <button class="rounded-full text-white bg-orange-700 px-6 py-1 hover:bg-orange-500">Go</button>
                    </div>
                </form>
                <div class="hidden md:block text-white">
                    Copyright &copy; 2025 Procash Chak.
                </div>
            </div>

        </div>
    </footer>
</template>
<style scoped> </style>