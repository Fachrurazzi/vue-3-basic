<template>
    <div>Ini adalah child component dasar</div>
    <div>{{ text }}</div>
</template>

<script>
export default {
    props: {
        text: {
            type: String, 
            default: ''
        }
    }
}
</script>