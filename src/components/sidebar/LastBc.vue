<script setup>
import IconBell from "../icons/IconBell.vue";
const timestamp = '13:37';
</script>

<template>
    <article class="last-bc margin--top-2 margin--bottom-1">
        <IconBell />
        <span>Last notification:</span>
        <span v-if=timestamp>{{ timestamp }}&nbsp;ECT</span>
    </article>
</template>
