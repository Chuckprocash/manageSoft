<script setup>
    import Testimonial from './TestimonialComponent.vue';
    import { ref } from 'vue';

    const cards = ref([
        {
            name: 'Alisha',
            avatar: 'avatar-1.jpg',
        },
        {
            name: 'Cidney',
            avatar: 'avatar-2.jpg',
        },
        {
            name: 'Jovany',
            avatar: 'avatar-3.jpg',
        },
    ]);

</script>
<template>
    <section class="testomonial">
        <div class="max-w-6xl mx-auto text-center px-5 mt-32">
            <h2 class="font-bold text-4xl text-center">
                What's Different About Manage?
            </h2>
            <div class="flex flex-col mt-10 md:flex-row md:space-x-6">
                <Testimonial v-for="card in cards" :key="card.name" :card="card" :class="card.name !== 'Alisha' ? 'hidden md:flex': ''"/>
            </div>
        </div>
    </section>
</template>
<style scoped>
</style>