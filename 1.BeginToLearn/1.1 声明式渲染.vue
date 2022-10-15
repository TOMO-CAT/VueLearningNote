<script>
// 导出默认模块, 外部可以直接使用 message 和 counter
export default {
    // 创建一个属性属性, 它包含 message 和 counter 两个成员
    data() {
        return {
            message: 'Hello World',
            counter: {
                count: 0
            }
        }
    }
}
</script>

<template>
    <h1>{{message}}</h1>
    <p>Count is: {{counter.count}}</p>
</template>