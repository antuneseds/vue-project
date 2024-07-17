<script setup></script>

<template>
    <div class="card">
        <div class="header">
            <slot name="header"></slot>
        </div>
        <slot>Corpo Padrão do Card</slot>
        <div v-if="$slots.footer" class="footer"></div>
        <div class="footer">
            <slot name="footer"></slot>
        </div>
    </div>
</template>

<style scoped>
    .card{
        height: 200px;
        width: 400px;
        box-shadow: 2px 2px 3px 3px gray;
    }

    .header {
        background-color: palevioletred;
        height: 60px;
        width: 100%;
        border-radius: 20px;
    }
</style>