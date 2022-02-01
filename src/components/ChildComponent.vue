<template>
    <div>Title</div>
    <slot :data="title"/>
    <div>Content</div>
    <slot name="content" :data="content"/>
    <div>Footer</div>
    <slot name="footer" :data="footer"/>
</template>

<script>
export default {
    data() {
        return {
            title:'Belajar Vue 3',
            content: 'Belajar Framework Vue 3',
            footer: 'copyright 2022'
        }
    }
}
</script>