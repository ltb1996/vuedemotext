<template>
    <div class="zuhemobanyingyong">
        <h3>组合式---模板引用</h3>
        <p ref="message">这是组合式模板引用的内容</p>
        <hr>
    </div>

</template>

<script setup>
import {ref, onMounted, watch} from 'vue';

const message = ref(null);

// 声明一个ref来存放该元素的引用， 必须和模板里的ref同名
// 如果想要更改dom里面的元素内容，则不能够放在最外层，因为在dom还有渲染的时候，这里的代码就已经执行
// 必须保证dom渲染完成之后再去读取dom

onMounted(() => {
    // console.log(message.value, '4545454545');
    message.value.style.color = 'Aqua';
    message.value.style.fontSize = '30px';
    message.value.innerHTML = '++++666665656565+++++';
});

</script>

<style scoped>
.zuhemobanyingyong{
  color: red;
}

</style>