<template>
    <div class="card" style="width: 18rem;">
        <div class="card-body">
            <h5 class="card-title">{{ title }}</h5>
            <h6 class="card-subtitle mb-2 text-body-secondary">{{ author }}</h6>
            <p class="card-text">{{ description }}</p>
            <a :href="img_url" class="card-link">link</a>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped></style>