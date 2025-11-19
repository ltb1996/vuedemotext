<template>
  <div class="use-pinia">
    <hr>
    <h3>pinia简单使用</h3>
    <p>计数：{{ counterStore.count }}</p>
    <button @click="counterStore.increment">增加</button>
    <p>双倍计数：{{ counterStore.doubleCount }}</p>
    <ul>
        <li v-for="(value, index) in counterStore.list.slice(0, 5)" :key="index">
            <p>{{ value.name }}</p>
            <img :src="value.img" :alt="value.name">
        </li>
    </ul>
  </div>
</template>

<script setup>
import { useCounterStore } from '../stores/counter';
import { onMounted } from 'vue';
const counterStore = useCounterStore();

console.log(counterStore, '5555555555555555555');

onMounted(() => {
    counterStore.getList();
});

</script>

<style scoped>
.use-pinia {
  color: aquamarine;
}
</style>
