<!-- eslint-disable vue/multi-word-component-names -->

<template>
    <span>{{ this.prefix + Number.parseFloat(this.value).toFixed(this.precision) }}</span>
</template>

<script>
export default {
    props: {
        value: Number, 
        prefix: {
            type: String,
            default: '$'
        },
        precision: {
            type: Number,
            default: 2
        }
    }
}
</script>