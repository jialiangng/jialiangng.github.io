<template>
    <h1 class="pt-5 pb-10">
        <span class="section-header text-4xl font-bold">
            <slot name="title"></slot>
        </span>
    </h1>
</template>

<script>
    export default {
        name: 'SectionTitle'
    }
</script>

<style>
.section-header {
  background: linear-gradient(90deg, white, gray);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-align: center;
  line-height: 1.2;
}
</style>