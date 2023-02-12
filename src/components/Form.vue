<template>
        <div>
        <h2>Meu Formulário</h2>
        <InputText /><br>
        <InputText /><br>
        <Submit />

        </div>
</template>

<script>
import InputText from './form/InputText.vue';
import Submit from './form/Submit.vue';

export default {
        name: 'Form',
        components: {
                InputText,
                Submit
        }
}
</script>