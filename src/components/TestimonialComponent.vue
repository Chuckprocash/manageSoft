<script setup>

const props = defineProps({
    card: {
        type: Object,
        required: true
    },
});

// console.log(props.card)
</script>
<template>
    <div class="flex flex-col items-center bg-gray-50 md:w-1/3 rounded-lg space-y-4 p-6">
                    <img        :src="`/images/${card.avatar}`" alt="image" class="max-w-[100px] rounded-full">
                    <h3 class="font-bold uppercase">{{ card.name }}</h3>
                    <small class="text-gray-700">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Atque beatae consequatur soluta, 
                    corporis blanditiis provident nulla </small>
    </div>
</template>
<style scoped></style>