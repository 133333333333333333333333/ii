<template>
  <div class="welcome">
   <div class="suibian">
      <h3>整个介绍吧</h3>
    <p>知道你们懒得看字直接上图耶</p>
   <p>不行还是悄咪咪看把</p>
      <button @click="showMe()">点我呗</button>
   </div>
   <img id="img" src="../../../assets/me.jpg" alt="" srcset="">
  </div>
</template>

<script>
export default {
  name: 'Welcome',
  methods: {
    showMe () {
      if (document.getElementById('img').style.display === 'block') {
        document.getElementById('img').style.display = 'none'
      } else {
        document.getElementById('img').style.display = 'block'
      }
    }
  }
}
</script>

<style lang="less" scoped>
.welcome {
  font-size: 20px;
  color: #8fd4af;
}
.suibian {
  margin-left: 20px;
}
img {
  width: 30%;
  height:30%;
  // margin: auto;
  border-radius: 5px;
  animation:my 5s infinite;
-webkit-animation:my 3s forwards;
  display: none;
}
@keyframes my {
  from {margin-left:0px;}
to {margin-left:400px;}
}
button {
  border: 6px solid #8fd4af;
  background-color: #8fd4af;
  color: rgb(136, 82, 12);
}

</style>
