<script setup>
const MultipliactionLength = 10;

</script>

<template>
    <div class="mx-auto max-w-screen-md ">
        <div v-for="number in MultipliactionLength" :key="number" class="flex space-x-2 mb-2">

            <div v-for="numberTwo = 1 in MultipliactionLength" :key="numberTwo" class="flex flex-col space-y-2 border border-gray-200 w-12 py-2">
                {{(number * numberTwo)}}
            </div>
        </div>
    </div>
</template>