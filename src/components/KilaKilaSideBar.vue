<template>
    <!-- 侧边栏 -->
    <div id="side-bar">
        <slot>
            <admin-card />
            <hot-article-card />
            <category-card />
            <tag-card />
            <archive-card />
        </slot>
    </div>
</template>

<script>
export default {
    name: "KilaKilaSideBar"
}
</script>

<style lang="less" scoped>
#side-bar {
    width: 26%;
    margin-right: 20px;
}

@media screen and (max-width: 900px) {
    #side-bar {
        display: none;
    }
}
</style>