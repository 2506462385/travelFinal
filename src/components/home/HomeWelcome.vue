<script setup>
import {ref} from "vue"

const msg = ref('欢迎访问旅游推荐站点');
const msg_en = ref('Welcome To The Recommended Tourist Sites')
</script>

<template>
  <div class="Hello">
    <h1>{{ msg }}</h1>
    <p style="color:#02b983"> {{ msg_en }}</p>
    <br>
    <p>
      你写PPT时，阿拉斯加的鳕鱼正跃出水面....
    </p>
    <p>
      你看报表时，梅里雪山的金丝猴刚好爬上树尖.....
    </p>
    <p>
      你挤进地铁时，西藏的山鹰一直盘旋云端....
    </p>
    <p>
      你在会议中时，尼泊尔的背包客一起端起酒杯坐在火堆旁....
    </p>
    <p>
      总有一些穿高跟鞋走不到的路，
    </p>
    <p>
      总有一些喷着香水闻不到的空气，
    </p>
    <p>
      总有一些在写字楼里却永远遇不见的人。
    </p>
  </div>
</template>


<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}


</style>
