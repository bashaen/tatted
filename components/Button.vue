<template>
    <button @click="onClick" :class="classes"><slot>Submit</slot></button>
</template>

<script>
export default {
    data () {
        return {
            "classes": ""
        }
    },
    props: {
        onClick: {
            type: Function,
            required: true
        }
    }
}
</script>
