<template>
  <div id="basicLayout">
    <a-layout style="height: 100vh">
      <a-layout-header class="header">
        <GlobalHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer">
        <a-space>
          <a href="https://github.com/LLLL1024" target="_blank">程序员兮颜</a>
          <a
            href="https://beian.miit.gov.cn"
            target="_blank"
            class="link-color-2"
            >ICP备案号：赣ICP备2024039351号-1</a
          >
        </a-space>
      </a-layout-footer>
    </a-layout>
  </div>
</template>

<script setup lang="ts">
import GlobalHeader from "@/components/GlobalHeader.vue";
</script>

<style scoped>
#basicLayout {
}

#basicLayout .header {
  margin-bottom: 16px;
  box-shadow: #eee 1px 1px 5px;
}

#basicLayout .content {
  box-sizing: border-box;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto 28px;
  padding: 20px;
  background: linear-gradient(to right, #fefefe, #fff);
}

.footer {
  padding: 16px;
  text-align: center;
  background: #efefef;
}

/* .link-color-1 {
  color: #00c8ff;
} */

.link-color-2 {
  color: #ff0000;
}
</style>
