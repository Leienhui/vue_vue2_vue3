<template>
  <h2>当前求和为：{{ sum }}</h2>
  <button @click="sum++">点我+1</button>
</template>

<script>
import {
  ref,
  onBeforeMount,
  onMounted,
  onBeforeUpdate,
  onUpdated,
  onBeforeUnmount,
  onUnmounted,
} from "vue";
export default {
  name: "Demo",
  // 在vue3中,生命周期钩子通过组合API的形式放到setup中时，setup就相当于beforeCreate和created，所以这两个钩子不能放到setup中
  setup() {
    console.log("---setup---");
    //数据
    let sum = ref(0);

    //通过组合式API的形式去使用生命周期钩子
    onBeforeMount(() => {
      // 挂载前执行
      console.log("---onBeforeMount---");
    });
    onMounted(() => {
      console.log("---onMounted---");
    });
    onBeforeUpdate(() => {
      console.log("---onBeforeUpdate---");
    });
    onUpdated(() => {
      console.log("---onUpdated---");
    });
    onBeforeUnmount(() => {
      console.log("---onBeforeUnmount---");
    });
    onUnmounted(() => {
      console.log("---onUnmounted---");
    });

    //返回一个对象（常用）
    return { sum };
  },
  //通过配置项的形式使用生命周期钩子，setup在beforeCreate之前执行
  //#region
  beforeCreate() {
    console.log("---beforeCreate---");
  },
  created() {
    console.log("---created---");
  },
  beforeMount() {
    console.log("---beforeMount---");
  },
  mounted() {
    console.log("---mounted---");
  },
  beforeUpdate() {
    console.log("---beforeUpdate---");
  },
  updated() {
    console.log("---updated---");
  },
  beforeUnmount() {
    console.log("---beforeUnmount---");
  },
  unmounted() {
    console.log("---unmounted---");
  },
  //#endregion

  //   总结：组合式API生命周期钩子的运行时期比配置项生命周期钩子快
  //   顺序：setup->beforeCreate->created->onBeforeMount->beforeMount....,但是一般情况下不会同时出现组合式API生命周期与配置项生命周期钩子
};
</script>
