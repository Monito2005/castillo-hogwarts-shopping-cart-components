<template>
    <div>
        <CartListItem v-for="item in cartItems" :key="item.id" :item="item"></CartListItem>
    </div>
</template>

<script setup>
import CartListItem from '@/components/CartListItem.vue'
defineProps(['cartItems'])
</script>

<style scoped></style>