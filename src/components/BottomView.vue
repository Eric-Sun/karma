<template>
  <div class="">
    <div class="bg-dark clear pt-20 pb-20 pl-20 pr-20">
      <Row :gutter="16" class="white">
        <Col :xs="{ span: 24}" :sm="{ span: 9}">
          <div>
            <Icon type="md-call" size="30"/>
            <span class="f-18">联系我们</span>
          </div>
          <div class="mt-25">地址：北京市朝阳区大鲁店街21号1层1123</div>
          <div class="mt-15">联系电话：18622615681</div>
        </Col>
        <Col :xs="{ span: 24}" :sm="{ span: 5}">
          <div class="" style="margin-top: 54px">邮箱：docsun.bo@gmail.com</div>
          <div class="mt-15">传真：-</div>
        </Col>
        <Col :xs="{ span: 24}" :sm="{ span: 5}">
          <div class="" style="margin-top: 54px">网址：https://cosydesign.cn</div>
          <div class="mt-15">邮编：100000</div>
        </Col>
      </Row>
    </div>
    <Divider style="margin: 0;background-color: #606b83;"/>
    <div class="tc white pt-10 pb-10 f-12">京ICP备17058409号-1</div>
  </div>
</template>

<script>
  export default {
    name: 'TopNav',
    data () {
      return {
        value: 0,
        autoplay: true,
        autoplaySpeed: 5000,
        loop: true,
        dots: 'outside',
        radiusDot: false,
        trigger: 'click',
        arrow: 'never'
      }
    },
    mounted () {

    },
    computed: {

    }
  }
</script>

<style scoped>
  .partner{
    padding: 40px 0;
    text-align: center;
  }
  .partner-item{
  }
  .partner-item img{
    border: 1px solid #dcdcdc;
    height: 60px;
    max-width: 80%;
    margin: 10px 8px 0;
  }
</style>
