<script>
export default {
    data() {
        return {
            titleClass: 'title'
        }
    }
}
</script>

<template>
    <!--
        Vue 中 mustache 语法(即双大括号)只能用于文本插值
        为了给 attribute 帮顶一个动态值, 需要使用 `v-bind` 指令:

        <div v-bind:id="dynamicId"></div>
        由于 v-bind 使用非常频繁, 因此它常常被简写成:
        <div :id="dynamicId"></div>
    -->

    <!-- 将一个动态 class 绑定添加到 <h1> 中, 并使用 titleClass 的数据属性作为它的值 -->>
    <h1 :class="titleClass"> Make me red</h1>
</template>

<style>
.title {
    color: red;
}
</style>