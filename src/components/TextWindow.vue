<template>
    <div class="text-window">
        <TextArea></TextArea>
        <TextArea></TextArea>
    </div>
</template>

<script>
import TextArea from './TextArea.vue'

export default {
    name: 'TextWindow',
    components: {
        TextArea
    }
}
</script>

<style scoped>
.text-window {
    /* 2vw accounts for status bar */
    height: calc(100% - 2vw);
    display: flex;
    justify-content: space-around;
}
</style>
