<template>
  <transition
    name="slide"
    enter-active-class="animated slideInRight"
    leave-active-class="animated slideOutRight"
  >
    <div class="menu" v-show="$parent.isMenu">
      <label>
      <h3>時間設定</h3>
        <p>
          番茄時光：
          <input type="number" value="25" /> 分鐘
        </p>
        <p>
          小歇時光：
          <input type="number" value="5" /> 分鐘
        </p>
        <p>
          休息時光：
          <input type="number" value="20" /> 分鐘
        </p>
      </label>
    </div>
  </transition>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style>
.menu {
  position: fixed;
  width: 30vw;
  height: 100vh;
  background-color: rgba(255, 255, 255, 0.99);
  right: 0;
  top: 0;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  z-index: -1;
  padding: 50px 20px 20px 20px;
}
svg {
  width: 30px;
  color: #fff;
  padding: 5px;
  position: relative;
  float: left;
  cursor: pointer;
}
h3 {
  font-weight: normal;
}
</style>
