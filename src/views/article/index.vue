<template>
    <div class="page">
        <div class="page-list">
            <article-list></article-list>
        </div>
        <div class="page-sidebar" id="sidebar">
            <sidebar-box title="文章标签" icon="tags" color="red">
                <sidebar-tags slot="list"></sidebar-tags>
            </sidebar-box>
            <sidebar-box title="作者榜" icon="tags">
                <sidebar-userlist slot="list"></sidebar-userlist>
            </sidebar-box>
        </div>
    </div>
</template>

<script>
    import ArticleList from "../../components/article/article-list";
    import SidebarBox from "../../components/sidebar/sidebar-box";
    import SidebarTags from "../../components/sidebar/sidebar-tags";
    import SidebarUserlist from "../../components/sidebar/sidebar-userlist";

    export default {
        name: 'index',
        components: {SidebarUserlist, SidebarTags, SidebarBox, ArticleList},
        mounted() {},
        methods: {}
    }
</script>

<style scoped lang="less">

</style>
