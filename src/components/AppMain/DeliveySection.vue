<script>
import { data } from '../../assets/data';
import ActionCall from '../generics/ActionCall.vue';
export default {
    name: 'DeliverySection',
    data() { return { data } },
    components: { ActionCall }
}
</script>
<template>
    <section id="delivery" class="d-flex jc-center ai-center pr-400">
        <action-call :label="data.delivery.label" :title="data.delivery.title" :button_label="data.delivery.button"
            class="ml-450"></action-call>
    </section>
</template>

<style lang="scss">
@use '../../assets/scss/partials/variables' as *;
@use '../../assets/scss/partials/mixins' as *;

#delivery {
    color: white;

    height: 530px;
    width: auto;

    background-image: url('../../assets/img/call-to-action-bg.jpg');
    @include bg-image;

    h2 {
        font-size: 2rem;
    }

    button {
        @include white-btn;

        &:hover {
            background-color: $violet2;
        }
    }
}
</style>