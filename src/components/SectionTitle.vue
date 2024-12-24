<template>
    <h1 class="w-5/6 lg:w-1/2 mx-auto bg-white mb-5 shadow-lg rounded-lg pt-3 pb-3 flex flex-row justify-center space-x-3">
        <slot name="icon"></slot>
        <span class="text-2xl lg:text-4xl">
            <slot name="title"></slot>
        </span>
    </h1>
</template>

<script>
    export default {
        name: 'SectionTitle'
    }
</script>