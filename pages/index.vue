<template>
  <div>
    <a-menu v-model="current" mode="horizontal">
      <a-menu-item key="article">
        <a-icon type="mail"/>
        我的文章
      </a-menu-item>

      <a-menu-item key="board">
        <a-icon type="appstore"/>
        留言板
      </a-menu-item>

      <a-sub-menu>
        <span slot="title" class="submenu-title-wrapper"
        ><a-icon type="setting"/>关于我</span
        >
        <a-menu-item-group title="Item 1">
          <a-menu-item key="setting:1">
            github
          </a-menu-item>
          <a-menu-item key="setting:2">
            语雀
          </a-menu-item>
        </a-menu-item-group>
      </a-sub-menu>

      <a-menu-item key="alipay">
        <a href="https://yuque.com/canal" target="_blank" rel="noopener noreferrer"
        >我的语雀</a
        >
      </a-menu-item>
    </a-menu>
  </div>
</template>
<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      current: ['mail'],
    };
  }
}
</script>
