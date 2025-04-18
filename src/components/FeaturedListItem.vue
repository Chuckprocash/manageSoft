<script setup>
 import { defineProps } from 'vue';

 const props = defineProps({
    item: {
        type: Object,
        required: true
    }
 });

//  console.log(props.item);

</script>
<template>
    <section>
        <div class="flex flex-col space-y-3 md:space-y-0 md:space-x-2 md:flex-row">
                    <div class="rounded-l-full bg-orange-300 md:bg-transparent ">
                        <div class="flex items-center space-x-2">
                            <div class="px-4 py-2 rounded-full bg-orange-700 text-white md:py-1">
                                {{ item.num }}
                            </div>
                            <h3 class="text-base font-bold md:hidden">
                                {{ item.title }}
                            </h3>
                        </div>
                    </div>
                    <div class="text">
                        <h3 class="text-base hidden font-bold md:block">{{ item.title }}</h3>
                        <p class="text-gray-800">
                           {{ item.text }}
                        </p>
                    </div>
                </div>
    </section>
</template>