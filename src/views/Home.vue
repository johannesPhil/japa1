<template>
  <div class="home">
    <div class="container">
      <div class="avatar">
        <img alt="Vue logo" src="../assets/IMG_3360.jpg" />
      </div>
      <h1>Hi there, my name is</h1>

      <MyName :myName="name" />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import MyName from "@/components/MyName.vue";

export default {
  name: "Home",
  components: {
    MyName
  },
  data() {
    return {
      name: "John Peter"
    };
  }
};
</script>

<style scoped>
.home {
  display: flex;
  justify-content: center;
  align-items: center;
}
.container {
  margin: 0;
  position: absolute;
  top: 50%;
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
  width: 300px;
  height: auto;
  margin: auto;
  padding: 5%;
  -webkit-box-shadow: -1px 0px 10px -1px rgba(198, 198, 198, 1);
  -moz-box-shadow: -1px 0px 10px -1px rgba(198, 198, 198, 1);
  box-shadow: -1px 0px 10px -1px rgba(198, 198, 198, 1);
}
.avatar {
  width: 200px;
  height: 200px;
  margin: auto;
  border-radius: 50%;
  overflow: hidden;
  -webkit-box-shadow: -1px 0px 10px -1px rgba(198, 198, 198, 1);
  -moz-box-shadow: -1px 0px 10px -1px rgba(198, 198, 198, 1);
  box-shadow: -1px 0px 10px -1px rgba(198, 198, 198, 1);
}

img {
  width: 100%;
  height: 100%;
}
</style>
