<script setup></script>
<template>
    <section>
        <nav class="container relative mx-auto p-6">
            <div class="flex items-center justify-between">
                <div class="pt-2 flex items-center ">
                    <img src="../assets/lion.svg" alt="Logo" class="h-[45px] w-[45px]" />
                    <a href="#"><span class="text-3xl font-semibold title-logo lowercase">Manage</span></a>
                </div>
                <div class="hidden md:flex space-x-6 pt-4">
                    <a class="hover:text-gray-600 " href="#">Product</a>
                    <a class="hover:text-gray-600" href="#">Pricing</a>
                    <a class="hover:text-gray-600" href="#">Careers</a>
                    <a class="hover:text-gray-600" href="#">Community</a>
                    <a class="hover:text-gray-600" href="#">About Us</a>
                </div>
                <a href="#" class="p-2 px-6 mt-3 text-white bg-orange-700 baseline rounded-full hidden md:block hover:bg-orange-600 transition duration-200">
                    Get Started
                </a>
            </div>
        </nav>
    </section>
</template>
<style scoped>
.title-logo{
    margin-left: -20px;
    line-height: 1em;
    transition: all 0.3s ease-in-out;
    font-family: 'Poppins', sans-serif;
}
.title-logo:hover{
    box-shadow: 0px 1px 0px #eee;
}
nav a{
    font-weight: 600;
}
</style>