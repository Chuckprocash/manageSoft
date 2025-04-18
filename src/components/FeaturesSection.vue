<script setup>
    import ListItem from './FeaturedListItem.vue';
    import { ref } from 'vue';

    const lists = ref([
        {
            num: '01',
            title: 'Track Company Wide Progress',
            text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, illum! Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus, natus'
        },
        {
            num: '02',
            title: 'Target industry through our AI insight',
            text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, illum! Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus, natus'
        },
        {
            num: '03',
            title: 'employee happiness curve',
            text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, illum! Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus, natus'
        }
    ]);
</script>
<template>
    <section class="features">
        <div class="container flex flex-col space-y-10 mx-auto px-4 mt-10 md:space-y-0 md:flex-row md:space-x-6">
            <div class="flex flex-col items-center space-y-10 md:w-1/2">
                <h2 class="max-w-md text-4xl text-center md:text-left font-bold">
                    What's Different About Manage
                </h2>
                <p class="max-w-sm text-center md:text-left text-gray-800">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quis, illum! Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus, natus.
                </p>
            </div>
            <div class="flex flex-col space-y-8 md:w-1/2">
                <!-- List Item 1 -->
                <ListItem v-for="list in lists" :item="list" :key="list.num"/>
            </div>
        </div>
    </section>
</template>
<style scoped>
</style>