<template>
  <div>
    <!--导航栏-->
    <Menu mode="horizontal" :theme="theme" :active-name="activeName" class="pl-20">
      <router-link tag="a" to="/" target="_blank"><img class="logo-pc" src="/static/img/logo.jpeg"></router-link>
      <div class="nav-pc" v-if="isPc">
      </div>
      <div class="fr mr-20" v-else>
        <Button type="primary" shape="circle" icon="ios-menu" @click="drawer = true"></Button>
      </div>
    </Menu>
  </div>
</template>

<script>
  export default {
    name: 'TopNav',
    props: {
      activeName: {
        type: String,
        default: '1'
      }
    },
    data() {
      return {
        theme: 'light',
        drawer: false,
        drawerTitle: '江西省产权交易中心',
        drawerWidth: '200',
        verticalMenuWidth: '200',
        value: 0
      }
    },
    mounted() {

    },
    computed: {
      isPc() {
        return this.$store.state.base.isPc
      }
    },
    methods: {
      selectDrawerMenu() {
        this.drawer = false
      }
    }
  }
</script>

<style scoped>
  .logo-pc {
    float: left;
    height: 40px;
    margin-top: 10px;
  }

  .nav-pc {
    float: right;
    height: 60px;
    line-height: 60px
  }
</style>
