<template>
    <div>
        <ProductDetails :product="product" />
    </div>
</template>

<script setup>
    const { id } = useRoute().params
    const uri = 'https://fuzik03.tetraserver.com/compactdisc?album=' + id

    // fetch singlle product
    const { data: product } = await useFetch(uri, { key: id})

    if(!product.value) {
        throw createError({ statusCode: 404, statusMessage: 'Product not found'})
    }

    definePageMeta({
        layout:'products'
    })
    
</script>

<style scoped>

</style>