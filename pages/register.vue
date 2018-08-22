<template>
  <section>
    <button-group></button-group>
    <template v-if="formType == 'FormLogIn'">
        <form-log-in></form-log-in>
    </template>
    <template v-if="formType == 'FormRegister'">
        <form-register></form-register>
    </template>
  </section>
</template>

<script>
import ButtonGroup from '~/components/ButtonGroup.vue'
import FormLogIn from '~/components/FormLogIn.vue'
import FormRegister from '~/components/FormRegister.vue'

export default {
    components: {
        ButtonGroup,
        FormLogIn,
        FormRegister
    },
    data () {
        return {
            formType: "FormLogIn"
        }
    }
}
</script>

<style>
.button-group {
    display: flex;
    margin: 0 auto;
    margin-top: 20px;
    width: 65%;
    border: 1px solid #d0d0d0;
}
.button {
    font-family: 'Aladin', sans-serif;
    font-size: 16px;
}
.button--action {
    padding: 5px 0;
    width: 50%;
    text-align: center;
}
.button--action.active {
    background: #ddd;
    border: none;
    font-style: italic;
}
.button--submit {
    background: #dedede;
    border: 1px solid #d3d3d3;
    display: block;
    margin: 0 auto;
    padding: 15px;
    width: 90%;
}
.title--default {
    background: none;
    border-bottom: 2px solid black;
    color: black;
    font-size: 36px;
    position: relative;
    top: 0;
}
</style>
