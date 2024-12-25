<template>
    <div class="skill-card">
        <div class="flex align-middle justify-center pb-10">
            <slot name="icon"></slot>
        </div>
        <div class="w-full">
            <div class="text-xl text-gray-400 rounded-lg p-2">
                <slot name="title"></slot>
            </div>
            <div class="flex flex-col pt-5">
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