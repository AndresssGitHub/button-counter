<script setup>
    import {ref} from 'vue'
    let count = ref(0);

    function addvalue(){
        count.value++;
        console.log(count)
    }
</script>

<template>
    <div @click="addvalue()" class="bg-green-500 w-30 h-10 px-4 py-2 rounded-md text-white font-semibold inline-block hover:cursor-pointer hover:bg-green-600 transition-colors">
        ¡Press me! {{ count }}
    </div>
</template>