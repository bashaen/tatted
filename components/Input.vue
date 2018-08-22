<template>
    <input :type="type" :placeholder="placeholder" :class="classes">
</template>

<script>
export default {
    data () {
        return {
            "placeholder": "",
            "type": "text",
            "classes": ""
        }
    }
}
</script>
