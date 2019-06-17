<template>
  <div class="layout">
    <layout>
      <header>
        <Menu mode="horizontal" theme="light">
          <div class="layout-logo"></div>
          <div class="layout-nav">
            <menu-item name="1">
              <icon type="ios-navigate"></icon>
              <span>Item 1</span>
            </menu-item>
            <menu-item name="2">
              <Icon type="ios-keypad"></Icon>
              Item 2
            </menu-item>
            <menu-item name="3">
              <Icon type="ios-analytics"></Icon>
              Item 3
            </menu-item>
            <menu-item name="4">
              <Icon type="ios-paper"></Icon>
              Item 4
            </menu-item>
          </div>
        </Menu>
      </header>
      <content :style="{padding: '0 50px'}">
        <breadcrumb :style="{margin: '20px 0'}">
          <breadcrumb-item>Home</breadcrumb-item>
          <breadcrumb-item>Components</breadcrumb-item>
          <breadcrumb-item>Layout</breadcrumb-item>
        </breadcrumb>
        <card>
          <div style="min-height: 200px;">
            Content
          </div>
        </card>
      </content>
      <footer class="layout-footer-center">2011-2016 &copy; TalkingData</footer>
    </layout>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      visible: false,
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    show: function () {
      this.visible = true
    }
  }
}
</script>
<style scoped>
  .layout{
    border: 1px solid #d7dde4;
    background: #f5f7f9;
    position: relative;
    border-radius: 4px;
    overflow: hidden;
  }
  .layout-logo{
    width: 100px;
    height: 30px;
    background: #5b6270;
    border-radius: 3px;
    float: left;
    position: relative;
    top: 15px;
    left: 20px;
  }
  .layout-nav{
    float: left;
    margin-left: 60px;
  }
  .layout-footer-center{
    text-align: center;
  }
</style>
