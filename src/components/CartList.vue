<template>
    <div>
        <CartListItem v-for="item in cartItems" :key="item.id" :item="item" @item-remove="$emit('item-remove', $event )" @quantity-update="$emit('quantity-update', $event)"></CartListItem>
    </div>
</template>

<script setup>
import CartListItem from '@/components/CartListItem.vue'
defineProps(['cartItems'])
defineEmits(['item-remove', 'quantity-update'])
</script>

<style scoped></style>