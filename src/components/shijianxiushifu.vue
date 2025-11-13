<template>
    <div class="shijianxiushifu">
        <h3>事件修饰符</h3>
        <!-- 阻止事件的默认行为 -->
        <a @click.prevent="click11" href="https://www.baidu.com">百度百度</a>

        <!-- 阻止事件冒泡 -->
        <div @click="clickDiv">
            <p @click.stop="clickP">测试冒泡</p>
        </div>
        

        <hr>
    </div>

</template>


<script>
export default {
    name: '8shijianxiushifu',
    data() {
        return {
        }
    },
    methods: {
        click11(e) {
            // e.preventDefault();
            console.log('点击了百度百度')
        },
        clickDiv() {
            console.log('点击了div')
        },
        clickP() {
            console.log('点击了p')
        }
    }
}

</script>


<style scoped>
.shijianxiushifu {
    color: slateblue;
}
</style>