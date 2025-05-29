<script lang="ts" setup>
import { computed, ref, onBeforeUnmount } from 'vue';

// create Reactive Date Object
const time = ref(new Date());
const updateInterval = setInterval(() => {
    time.value = new Date()
}, 1000);

// Computed functions to get units
const getSeconds = computed(() =>
    time.value.getSeconds().toString().padStart(2, '0'),
);
const getMinutes = computed(() =>
    time.value.getMinutes().toString().padStart(2, '0'),
);
const getHours = computed(() =>
    time.value.getHours().toString().padStart(2, '0'),
);

onBeforeUnmount(() => clearInterval(updateInterval));
</script>

<template>
    <div class="clock" role="presentation">
        [&nbsp;{{getHours}}:{{getMinutes}}:{{getSeconds}}&nbsp;ECT&nbsp;]
    </div>
</template>