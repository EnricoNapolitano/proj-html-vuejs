<script>
import { data } from '../../assets/data/index';
import ActionCall from '../generics/ActionCall.vue';
export default {
    name: 'HeroJumbo',
    data() { return { data } },
    components: { ActionCall }
}
</script>

<template>
    <section id="hero-jumbo" class="d-flex ai-center">
        <div class="hero-call">
            <action-call :label="data.jumbo.label" :title="data.jumbo.title" :paragraph="data.jumbo.paragraph"
                :button_label="data.jumbo.button"></action-call>
        </div>
    </section>
</template>

<style lang="scss">
@use '../../assets/scss/partials/variables' as *;
@use '../../assets/scss/partials/mixins' as *;

#hero-jumbo {
    height: 750px;
    width: auto;
    background-image: url('../../assets/img/hero-header-bakery.jpg');
    @include bg-image;

    .hero-call {
        margin: 0 120px;
    }

    h2 {
        font-size: 55px;
    }

    button {
        @include white-btn;

        &:hover {
            background-color: $violet2;
        }
    }
}
</style>