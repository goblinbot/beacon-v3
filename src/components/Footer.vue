<script setup>
import DateCard from './footer-cards/Date.vue';
</script>

<template>
    <section class="footer">


        <DateCard />

        <article class="block block--chipped flex--6">
            
            <div class="block__content">
                <h2>Alert level</h2>
            </div>
        </article>
        
        <article class="block block--chipped flex--3">
            <div class="block__header">
                <h3>Open Connections</h3>
            </div>
            <div class="block__content">
                <p>:O</p>
                <p>112</p>
            </div>
        </article>

        <article class="block block--chipped flex--10">
            <div class="block__header">
                <h3>Operators & Workload | Connection info</h3>
            </div>
        </article>

        <article class="block block--chipped flex--1">
            [cog]
        </article>

    </section>
</template>