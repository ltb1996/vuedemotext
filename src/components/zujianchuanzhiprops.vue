
<template>
  <div class="zujianchuanzhiprops">
    <hr>
    <h3>组件传值（父传子）props</h3>
    <Child :message="message" :age="age" :names="names" :userInfo="userInfo"></Child>
    <!-- <hr> -->
    <!-- 注意事项：props传递数据，只能从父级传到子级，不能从子级传到父级，字符串，数字，数组，对象 -->
  </div>
</template>

<script>
import Child from '../pages/child.vue';
export default {
    name: 'zujianchuanzhiprops',
    data() {
        return {
            message: '父组件传值给子组件',
            age: 18,
            names: ['张三', '李四', '王五'],
            userInfo: {
                title: '78978797889',
                id: 4545
            }
        }
    },
    components: {
        Child
    }
};
</script>

<style scoped>
.zujianchuanzhiprops {
    color: yellow;
}
</style>
