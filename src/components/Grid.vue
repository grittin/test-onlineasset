<script>
export default {
  data() {
    return {
      datas: {},
    };
  },
  mounted() {
    let fetchRes = fetch(
      "https://demotrade.efintradeplus.com/ExamAPI/examdata"
    );
    fetchRes
      .then((res) => res.json())
      .then((d) => {
        this.datas = d;
      });
  },
};
</script>
<template>
  <div class="min-h-screen grid grid-rows-4 grid-flow-col gap-3">
    <div class="row-span-2 col-span-1 bg-red-200" >{{datas.data_1}}</div>
    <div class="row-span-1 col-span-1 bg-purple-200">{{datas.data_3}}</div>
    <div class="row-span-1 col-span-2 bg-yellow-200">{{datas.data_6}}</div>
    <div class="row-span-2 bg-green-200">{{datas.data_2}}</div>
    <div class="row-span-1 bg-blue-200">{{datas.data_4}}</div>
    <div class="row-span-4 col-span-1 bg-purple-300">{{datas.data_5}}</div>
  </div>
</template>