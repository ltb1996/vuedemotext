<!--
 * @Author: ltb1996 610030835@qq.com
 * @Date: 2025-10-09 16:35:17
 * @LastEditors: ltb1996 610030835@qq.com
 * @LastEditTime: 2025-11-06 08:19:46
 * @FilePath: \vuedemotext\src\views\home.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
    <div class="home-container">
        <h1>VUE3教学</h1>
        <hr>
        <Mobanyufa></Mobanyufa>
        <Shuxingbangding></Shuxingbangding>
        <Tiaojianxuanran></Tiaojianxuanran>
        <Liebiaoxuanran></Liebiaoxuanran>
        <Keyguanlizhuangtai></Keyguanlizhuangtai>
        <Shijianchuli></Shijianchuli>
        <Shijianchuancan></Shijianchuancan>
        <Shijianxiushifu></Shijianxiushifu>
        <Shuzubianhuazhence></Shuzubianhuazhence>
        <Jisuanshuxing></Jisuanshuxing>
        <Classbangding></Classbangding>
        <Stylebangding></Stylebangding>
        <Watchzhenting></Watchzhenting>
        <Biaodanshujvbangding></Biaodanshujvbangding>
        <Mobanyinyong></Mobanyinyong>
        <Zujianzucheng></Zujianzucheng>
        <Zujianqiantao></Zujianqiantao>
    </div>
</template>

<script>
import Mobanyufa from '../components/mobanyufa.vue';
import Shuxingbangding from '../components/shuxingbangding.vue';
import Tiaojianxuanran from '../components/tiaojianxuanran.vue';
import Liebiaoxuanran from '../components/liebiaoxuanran.vue';
import Keyguanlizhuangtai from '../components/keyguanlizhuangtai.vue';
import Shijianchuli from '../components/shijianchuli.vue';
import Shijianchuancan from '../components/shijianchuancan.vue';
import Shijianxiushifu from '../components/shijianxiushifu.vue';
import Shuzubianhuazhence from '../components/shuzubianhuazhence.vue';
import Jisuanshuxing from '../components/jisuanshuxing.vue';
import Classbangding from '../components/classbangding.vue';
import Stylebangding from '../components/stylebangding.vue';
import Watchzhenting from '../components/watchzhenting.vue';
import Biaodanshujvbangding from '../components/biaodanshujvbangding.vue';
import Mobanyinyong from '../components/mobanyinyong.vue';
import Zujianzucheng from '../components/zujianzucheng.vue';
import Zujianqiantao from '../components/zujianqiantao.vue';

export default {
  name: 'home',
  components: {
    Mobanyufa,
    Shuxingbangding,
    Tiaojianxuanran,
    Liebiaoxuanran,
    Keyguanlizhuangtai,
    Shijianchuli,
    Shijianchuancan,
    Shijianxiushifu,
    Shuzubianhuazhence,
    Jisuanshuxing,
    Classbangding,
    Stylebangding,
    Watchzhenting,
    Biaodanshujvbangding,
    Mobanyinyong,
    Zujianzucheng,
    Zujianqiantao,
  },
}

</script>


<style scoped>
.home-container{
    position: relative;
    z-index: 10;
}

h1 {
    z-index: 11;
    color: aqua;
}
    
</style>