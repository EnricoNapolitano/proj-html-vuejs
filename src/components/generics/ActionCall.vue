<script>
export default {
    name: 'ActionCall',
    props: { label: String, title: String, paragraph: String, button_label: String }
}
</script>

<template>
    <div class="h-event">
        <h4 v-if="label">{{ label }}</h4>
        <h2 v-if="title">{{ title }}</h2>
        <p v-if="paragraph">{{ paragraph }}</p>
        <button v-if="button_label" class="btn">{{ button_label }}</button>
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as*;

div {
    max-width: 530px;
}

h4,
h2,
p {
    padding-bottom: 35px;
}

h2 {
    font-size: 25px;
}

p {
    line-height: 30px;
}
</style>