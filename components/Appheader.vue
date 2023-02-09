<template>
  <div class="d-flex header-div">
    <img src="/img/logo.png" alt="udemy" width="105px" height="51px">
    <div class="category-text">Categories</div>
    <div class="d-flex search-div">
      <img src="/img/icon-search.png" width="25px" height="25px" alt="">
      <input type="text" value="Search for Everything" class="border-none outline-none">
    </div>
    <h3 class="header-text2">Teach on Udemy</h3>
    <img src="/img/icon-cart.png" alt="" width="32px" height="auto" class="cart-
    icon">
    <button class="login-button">Login</button>
    <button class="signup-button">Sign up</button>
    <div class="world-icon">
      <img src="/img/world.png" width="20px" height="auto" alt="">
    </div>
  </div>
</template>
<script lang="ts">
</script>


<style lang="postcss">
.d-flex {
  display: flex;
  flex-direction: row;
}

.header-div {
  padding-left: 20px;
  padding-right: 20px;
  align-items: center;
}

.category-text {
  padding: 0 10px 0 10px;
}

.search-div {
  flex: 1;
  padding: 10px;
  border: 1px solid black;
  border-radius: 30px;
}

.search-icon {
  padding: 0 10px 0 10px;
}

.border-none {
  border: none;
}

.outline-none {
  outline: none;
}

.header-text2 {
  padding: 0 20px 0 20px;
}

.cart-icon {
  padding: 0 8px 0 2px;
}

.login-button {
  padding: 10px 20px 10px 20px;
  background: white;
  border: 1px solid;
  border-bottom: 1px solid #363636;
}

.signup-button {
  padding: 10px 20px 10px 20px;
  background: black;
  color: white;
  margin-left: 7px;
  border: 1px solid;
  border-bottom: 1px solid #363636;
}

.world-icon {
  padding: 5px;
  border: 1px solid black;
  margin-left: 7px;
}
</style>

<script lang="ts">
</script>