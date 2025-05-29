<script setup>
defineProps({
    title: {
        type: String,
        required: true,
    },
    status: {
        type: String,
        required: true,
    },
    // icon: {
    //     type: String,
    //     required: true,
    // },
    statusClass: {
        type: String,
        required: true,
    }
})
</script>

<template>
    <article class="status-tab" v-bind:class=statusClass>
        <div class="status-tab__title">{{ title }}</div>
        <div class="status-tab__content">{{ status }}</div>
        <!-- icon -->
    </article>
</template>