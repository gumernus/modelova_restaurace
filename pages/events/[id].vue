<script setup>

const route = useRoute();
console.log(route.fullPath);
console.log(route.params);

const nuxtApp = useNuxtApp();
console.log(nuxtApp);
</script>

<template>

    <div>
        event id: {{ $route.params.id }}
    </div>

</template>