<script>
export default {
    name: 'NavMenu',
    props: { menu: Array }
}
</script>

<template>
    <ul>
        <li v-for="item in menu" :key="item">
            <a href="#">{{ item }}</a>
        </li>
        <li>
            <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
        </li>
    </ul>
</template>

<style lang="scss" scoped>
ul {
    display: flex;
}

li {
    padding: 5px;
}
</style>