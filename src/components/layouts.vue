<template>
  <section class="container" > <!--最外层容器-->
    <section class="menu"> <!--左边的容器-->
      <menus></menus>
    </section>
    <section class="content-container"><!--右边的容器-->
      <todo></todo>
    </section>
  </section>
</template>
<script>
import menus from './menus';
import todo from './todo';
export default {
    components: {
        menus,
        todo
    }
}
</script>
<style lang = "less" scoped>
/* lang 指额外表示支持的语言可以让编辑器识别,scoped 指这里写的css只适用于该组件 */
@import '../common/style/layouts.less';
</style>