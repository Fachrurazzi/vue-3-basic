<template>
    <div>
        <span>Ini adalah child</span>

        <button @click="onPress">Click dari Child</button>
    </div>
</template>

<script>
export default {
    emits: ["child-click"],
    methods: {
        onClick() {
            console.log('click saya')
        },
        onPress() {
            this.$emit('child-click', 'value');
        }
    }
}
</script>