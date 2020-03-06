<template>
  <div class="container">
    <div class="home">
      <span class="home-element">Home</span>
      <span>&#62;</span>
      <span class="home-element">Tracking</span>
      <span>&#62;</span>
      <span class="home-element">Delivery Details</span>
    </div>
    <div class="consignment flex flex-row justify-between">
      <span class="consignment-title">Consignment Id</span>
      <div>
        <span class="consignment-id">{{ order.id }}</span>
        <img class="consignment-img" src="../assets/resource/ic_copy.svg" />
      </div>
    </div>
    <div class="shipping flex flex-row justify-between">
      <div class="shipping-title w-1/4">
        <p>Shipping Info</p>
      </div>
      <div class="shipping-info w-1/2">
        <p class="shipping-contact">{{ user.phone }}</p>
        <div class="shipping-address">
          <p>{{user.name}}</p>
          <p>{{ user.address}}</p>
        </div>
      </div>
    </div>
    <div class="timeline">
      <p class="timeline-title">Timeline</p>
      <div class="timeline-img"></div>
      <div class="timeline-details flex-col">
        <div class="item">
          <p class="title">Your order has been picked-up!</p>
          <p class="time">March 1,2020,10:00</p>
        </div>
        <div class="item">
          <p class="title">Our delivery man is on his way to pick up your order.</p>
          <p class="time">March 1,2020,10:00</p>
        </div>
        <div class="item">
          <p class="title">Your Order has been confirmed!</p>
          <p class="time">March 1,2020,10:00</p>
        </div>
        <div class="item">
          <p class="title">Your Order has been confirmed!</p>
          <p class="time">March 1,2020,10:00</p>
        </div>
        <div class="item">
          <p class="title">Your Order has been confirmed!</p>
          <p class="time">March 1,2020,10:00</p>
        </div>
      </div>
      <div class="load-more">
        <img src="../assets/resource/ic_down_arrow.svg" class="load-more-icon" />
        <span class="load-more-title">Load more</span>
      </div>
    </div>
    <div class="product flex flex-row justify-between">
      <div class="w-1/2 product-description">
        <p class="product-title">Product Description</p>
        <div class="product-list">
          <p class="item">01 Black Tshirt</p>
          <p class="item">02 Knee Guard</p>
        </div>
      </div>
      <div class="w-1/2 receipt">
        <p class="receipt-title">Receipt</p>
        <div class="receipt-details">
          <div class="element flex flex-row justify-between">
            <p class="element-name">Product price</p>
            <p>&#2547; 700</p>
          </div>
          <div class="element flex flex-row justify-between">
            <p class="element-name">Delivery Charge</p>
            <p>&#2547; 60</p>
          </div>
          <p class="element dotted-separator"></p>
          <div class="element flex flex-row justify-between">
            <p class="total">Total</p>
            <p class="total-price">&#2547; 600</p>
          </div>
        </div>
      </div>
    </div>
    <div class="merchant">
      <p class="merchant-title">Seller Info</p>
      <div class="merchant-info flex flex-row items-center">
        <img src="../assets/resource/logo.png" class="merchant-logo" />
        <div class="merchant-details">
          <p class="merchant-name">{{merchant.name}}</p>
          <p class="merchant-description">{{ merchant.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      order: {
        id: 64578912345
      },
      user: {
        name: "Shamsuddin Chowdhury Delwar",
        phone: "01654789123",
        address:
          "Genetic Baro Bhuiyan,kamal Ataturk Avenue,Gulshan 2,Dhaka 1213"
      },
      merchant: {
        name: "Abibas apparels joy endless",
        description: "Tshirt, panjabi, Men's wear"
      }
    };
  }
};
</script>
<style></style>
