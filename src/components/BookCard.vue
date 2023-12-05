<template>
    <div class="card" style="width: 18rem;">
        <div class="card-body">
            <h5 class="card-title">{{ konyv.title }}</h5>
            <h6 class="card-subtitle mb-2 text-body-secondary">{{ konyv.author }}</h6>
            <p class="card-text">{{ description }}</p>
            <a :href="konyv.img_url" class="card-link">link</a>
        </div>
    </div>
</template>

<script setup>
defineProps(["konyv"])
</script>

<style lang="scss" scoped></style>