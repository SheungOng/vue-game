<template>
    <button @click="onClick" class="Button">
        <slot>Button text</slot>
    </button>
</template>
<script>
export default {
    props: {
        onClick: {
            type: Function,
            required: true
        }
    }
}
</script>