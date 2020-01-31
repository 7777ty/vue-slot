# 如何使用slot？
  假设现有组件Layout.vue:
```vue
<template>
    <div class="nav-wrapper">
        <div class="content">
            <slot></slot>
        </div>
        <Nav/>
    </div>
</template>

<script lang='ts'>
    export default {
        name: 'Layout'
    };
</script>

<style lang='scss' scoped>

</style>
```

slot插槽处即是用于放置用户用户传入的内容用户内容通过以下形式传入：
```vue
<template>
    <Layout>Money</Layout>
</template>

<script lang='ts'>
    export default {
        name: 'Money2'
    };
</script>

<style lang='scss' scoped>

</style>
```