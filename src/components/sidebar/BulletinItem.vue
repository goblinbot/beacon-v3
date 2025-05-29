<script setup>
defineProps({
    timestamp: {
        type: String,
        required: true,
    },
    msg: {
        type: String,
        required: true,
    },
    author: {
        type: String,
        required: true,
    },
})
</script>

<template>
    <li class="bulletin__item">

        <span class="bulletin__timestamp">[{{ timestamp }}]</span>
        <span class="bulletin__post">
            <p>{{ msg }}</p>
            <p class="bulletin__author">-{{ author }}</p>
        </span>

    </li>
</template>