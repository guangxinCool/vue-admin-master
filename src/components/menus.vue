<template>
  <div class="list-todos">  <!--菜单容器-->
      <a class="list-todo activeListClass list" v-for="item in items"> <!--单个菜单容器-->
        <span class="icon-lock" v-if="item.locked"></span>
        <span class="count-list" v-if="item.count">{{item.count}}</span>
        {{item.title}}
      </a>
      <a class=" link-list-new" > <!--新增菜单-->
        <span class="icon-plus"></span>新增
      </a>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        items: [
          { title: '星期一', count: 1, locked: true},
          { title: '星期二', count: 1, locked: true},
          { title: '星期三', count: 1, locked: true},
          { title: '星期四', count: 1, locked: true},
          { title: '星期五', count: 1, locked: true},
          { title: '星期六', count: 1, locked: true},
          { title: '星期日', count: 1, locked: true}
        ]
      }
    }
  };
</script>
<style lang="less">
@import '../common/style/menu.less';
</style>