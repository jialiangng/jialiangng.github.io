<template>
    <div class="skill-card">
        <slot name="icon"></slot>
        <div class="bg-white p-5 rounded-lg shadow-sm w-4/5 lg:w-full">
            <div class="text-xl border-2 border-gray-400 rounded-lg px-2 py-1">
                <slot name="title"></slot>
            </div>
            <div class="flex flex-col mt-5">
                <slot name="content"></slot>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
    name: 'SectionComponent'
    }
</script>