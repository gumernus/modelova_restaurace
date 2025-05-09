<template>
    <div>
        <Main-PageNavbar />
        <section class="all-gallery">
            <h1>Všechny Fotky</h1>
            <div class="gallery-grid">
                <img v-for="image in images" :key="image" :src="`/gallery/${image}`" class="gallery-item" />
            </div>
        </section>
        <Main-PageFooter />
    </div>
</template>

<script setup>
const images = [
    'image-23.png',
    'image-34.png',
    'image-23.png',
    'image-34.png',
    'image-23.png',
    'image-34.png',
    'image-23.png',
    'image-34.png',
    'image-23.png',
    'image-34.png',
    'image-23.png',
    'image-34.png',
];
</script>

<style scoped>
.all-gallery {
    margin-top: 50px;
}

.gallery-grid {
    margin-top: 50px;
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* 3 images per row by default */
    gap: 25px;
}

.gallery-item {
    width: 100%;
    aspect-ratio: 1 / 1; /* Ensures all images are square */
    border-radius: 25px;
    object-fit: cover;
}

@media (max-width: 800px) {
    .gallery-grid {
        grid-template-columns: repeat(2, 1fr); /* 2 images per row for medium devices */
    }
}

@media (max-width: 500px) {
    .gallery-grid {
        grid-template-columns: 1fr; /* 1 image per row for small devices */
    }
}
</style>
