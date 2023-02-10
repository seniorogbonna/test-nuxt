<template>
  <div class="position-fixed right-side-card-section">
    <div class="d-flex align-items-center">
      <img src="/img/pound-icon.png" style="width:23px;height:19px;margin-top:3px;" alt="">
      <h2>44.99</h2>
    </div>
    <button class="w-full bg-purple cart-button">Add to cart</button>
    <button class="w-full buy-button font-bold">Buy Now</button>
    <p style="text-align: center;">30-Day Money-Back Guarantee</p>
    <h3>This course includes: </h3>
    <div class="d-flex align-items-center" style="padding: 6px">
      <img src="/img/video-icon.png" width="16px" height="16px" alt="">
      <span class="ml-3">19 hours on-demand video</span>
    </div>
    <div class="d-flex align-items-center" style="padding: 6px">
      <img src="/img/lifetime-icon.png" width="16px" height="16px" alt="">
      <span class="ml-3">Full lifetime access</span>
    </div>
    <div class="d-flex align-items-center" style="padding: 6px">
      <img src="/img/iphone-icon.png" width="16px" height="16px" alt="">
      <span class="ml-3">Access on mobile and TV</span>
    </div>
    <div class="d-flex align-items-center" style="padding: 6px">
      <img src="/img/trophy-icon.png" width="16px" height="16px" alt="">
      <span class="ml-3">Certificate of completion</span>
    </div>
    <div class="d-flex justify-content-between line-group" style="padding: 10px;">
      <a class="text-black font-bold" href="">Share</a>
      <a class="text-black font-bold" href="">Gift this course</a>
      <a class="text-black font-bold" href="">Apple coupon</a>
    </div>
    <h3 class="border-top" style="padding-left: 10px; margin-top: 30px; padding-top: 20px;">Training 5 or more people?
    </h3>
    <p style="padding: 10px;">Get your team access to 19,000+ top Udemy courses anytime, anywhere.</p>
    <button class="try-button">Try Udeny business</button>

  </div>
</template>

<style lang="postcss">
.position-fixed {
  position: fixed;
}

.right-side-card-section {
  width: 25%;
  background-color: white;
  right: 5%;
  top: 9%;
  border: 1px solid;
  padding: 10px 20px 10px 20px;
}

.bg-purple {
  background-color: #a435f0;
}

.cart-button {
  font-size: 24px;
  padding: 11px;
  color: white;
}

.text-black {
  color: black;
}

.buy-button {
  margin-top: 10px;
  font-size: 24px;
  padding: 11px;
  color: black;
  background-color: white;
}

.link-group {
  padding: 10px 0 10px 10px;
}

.try-button {
  margin-top: 10px;
  font-size: 20px;
  padding: 11px;
  color: black;
  background-color: white;
  width: 100%;
  font-weight: bold;
}
</style>