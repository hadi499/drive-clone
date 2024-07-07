<template>
    <div class="w-[600px] h-[80px] flex items-center">
        <TextInput type="text"
                   class="block w-full mr-2"
                   v-model="search"
                   autocomplete                  
                   placeholder="Search for files and folders"/>
    </div>
</template>

<script setup>
import TextInput from "@/Components/TextInput.vue"
import {router, useForm} from "@inertiajs/vue3"
import {onMounted, ref} from "vue";

const form = useForm({
    search: ''
})

</script>