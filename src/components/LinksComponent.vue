<template>
    <div class="flex space-x-1">
        <a href="https://www.linkedin.com/in/jia-liang-ng-2a2018260" target="_blank"
            class="linkbutton">LinkedIn
        </a>
        <a href="https://github.com/CyanKelv" target="_blank"
            class="linkbutton">Github
        </a>
    </div>
</template>

<script>
export default {
    name: 'LinksComponent'
}
</script>

<style>
.linkbutton{
    @apply px-1 py-1 rounded-md text-gray-400 hover:bg-gray-500 hover:text-white transition duration-300 md:px-4;
}
</style>