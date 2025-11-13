<template>
    <div class="zuhexiangyingshi">
        <h3>组合式API--响应式</h3>
        <p>{{ msg }}</p>
        <p>{{ asas }}</p>
        <p>{{ state.ok ? "ok1" : "ok2"}}</p>
        <p>{{ msg.split('').reverse().join('') }}</p>
        <p>{{ state.rawHtml }}</p>
        <p v-html="state.rawHtml"></p>
        <hr>
    </div>
</template>

<script setup>
import {ref, reactive} from 'vue';
/*
ref定义的是基本的数据类型：string number bollean
reactive定义的是引用类型的数据类型: object array
注意事项：两种写法尽量不要混在一起，尤其是写多个的子组件的时候，一个vue文件只能有一种写法
要么选项api,要么组合式api
*/
const msg = ref('hello world');
const asas = ref(12222);

const state = reactive({
    ok: true,
    rawHtml: "<a href = 'https://www.baidu.com'>百度</a>"
});
</script>

<style scoped>
.zuhexiangyingshi {
    color: yellow;  
}
</style>