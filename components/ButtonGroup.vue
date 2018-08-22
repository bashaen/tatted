<template>
    <div class="button-group">
        <v-button
            v-for="(button, index) of buttonList"
            v-bind:button="button"
            v-bind:key="index"
            v-bind:text="button.text"
            v-bind:class="button.class"
            v-bind:onClick="buttonClick"
            >{{ button.text }}</v-button>
    </div>
</template>

<script>
import VButton from '~/components/Button.vue'

export default {
    components: {
        VButton
    },
    data () {
        return {
            buttonList: [
                {
                    "class": "button button--action button--log-in active",
                    "formType": "FormLogIn",
                    "text": "Sign In"
                },
                {
                    "class": "button button--action button--sign-up",
                    "formType": "FormRegister",
                    "text": "Sign Up"
                }
            ]
        }
    },
    methods: {
        buttonClick: function(e) {
            var active = document.querySelector('button.active');
            active.classList.remove('active');
            e.target.classList.add('active');
            formType = this.formType;
        }
    }
}
</script>