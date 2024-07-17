<script setup> </script>

<template>
    <div class="card">
        <h3>IFC</h3>
        <slot></slot>
    </div>
</template>

<style scoped>
.card {
    height: 600px;
    width: 400px;
    border: 1px solid black;
    border-radius: 20px;
    box-shadow: 2px 2px 3px 3px gray;
}
</style>