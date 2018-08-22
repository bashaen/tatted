<template>
    <form action="" class="form form--sign-in">
        <v-input
            v-for="(input, index) in inputList"
            v-bind:input="input"
            v-bind:key="index"
            v-bind:type="input.type"
            v-bind:placeholder="input.placeholder"
            v-bind:class="input.class"
            ></v-input>
    </form>
</template>

<script>
import VInput from '~/components/Input.vue'

export default {
    components: {
        VInput
    },
    data () {
        return {
            inputList: [
                {
                    "class": "input--default",
                    "placeholder": "Username",
                    "type": "text"
                },
                {
                    "class": "input--default",
                    "placeholder": "Password",
                    "type": "password"
                }
            ]
        }
    }
}
</script>

<style>
</style>
