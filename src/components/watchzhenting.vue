<template>
    <div class="watchzhenting">
        <hr>
        <h3>watch监听</h3>
        <p>
            {{ message }}
        </p>
        <button @click="update">修改数据</button>
    </div>
</template>


<script>
export default {
    name: '13watchzhenting',
    data() {
        return {
            message: 'watchzhenting'
        }
    },
    methods: {
        update() {
            this.message = '11111111111111111update';
        }
    },
    watch: {
        //watch里面de函数名称必须与data中的属性名称相同，newValue是修改后的值，oldValue是修改前的值，这两个都是参数，是必须的
        message(newValue, oldValue){
            // 数据发生变化，自动执行的函数
            console.log(newValue, '+++++++++++');
            console.log(oldValue, '+---------------');
        }
    }

}

</script>

<style scoped>
.watchzhenting {
    color: blueviolet;
}
</style>