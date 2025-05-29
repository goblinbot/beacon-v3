<script setup>
import StatusTab from "./sidebar/StatusTab.vue"
import LastBc from "./sidebar/LastBc.vue"
import BulletinBoard from "./sidebar/BulletinBoard.vue"
</script>

<template>
    <section class="sidebar">

        <StatusTab title="PORTAL" status="Operational" statusClass="default" />

        <StatusTab title="CANOPY" status="OFFLINE" statusClass="disrupted" />

        <StatusTab title="TRINARY" status="Datastream Active" statusClass="default" />

        <BulletinBoard />

        <LastBc />

    </section>
</template>