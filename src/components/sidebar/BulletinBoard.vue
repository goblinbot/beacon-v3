<script setup>
import IconMMI from "../icons/IconMMI.vue";
import BulletinItem from "./BulletinItem.vue"
</script>

<template>
    <section class="bulletin">
        <header class="bulletin__header">
            <h2>
                <IconMMI /> Colony Feed : IPC_0661
            </h2>
        </header>

        <ul class="bulletin__feed">

            <BulletinItem timestamp="11:30" msg="COLONY MEETING @ 12:45" author="Military Coolguy"/>
            <BulletinItem timestamp="11:31" msg="NEVER MIND" author="Military Coolguy"/>

            <BulletinItem timestamp="12:48" msg="Where is everyone" author="Steampunk Cosplayer"/>
            <BulletinItem timestamp="12:53" msg="Where do we meet" author="Milkshake Pilot"/>

            <BulletinItem timestamp="12:53" msg="Comprehensive reading & you: a Guide. Please." author="ADMINFOMORPH"/>

            <BulletinItem timestamp="12:55" msg="🍆" author="🍆" />
        </ul>

    </section>
</template>