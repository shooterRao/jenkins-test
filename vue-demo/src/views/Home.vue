<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Hello Jenkins!!!!!!"/>
    <SvgIcon iconClass="icon-peradd"/>
    <SvgIcon iconClass="icon-star"/>
    <SvgIcon iconClass="icon-loading"/>
    <SvgIcon iconClass="icon-sousuo"/>
    <SvgIcon iconClass="icon-refresh"/>
    <SvgIcon iconClass="icon-item"/>
    <div>
      <SvgIcon iconClass="icon-peradd"/>
      <span style="margin-left: 5px">用户名</span>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import SvgIcon from "@/components/SvgIcon.vue"
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
    SvgIcon
  }
}
</script>
