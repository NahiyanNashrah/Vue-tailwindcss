<template>
  <div class="container">
    <div class="home">
      <span class="home-element">Home</span>
      <img src="../assets/resource/symbol.svg" alt class="home-icon" />
      <span class="home-element">Tracking</span>
      <img src="../assets/resource/symbol.svg" alt class="home-icon" />
      <span class="home-element">Delivery Details</span>
    </div>
    <div class="consignment">
      <p class="consignment-title">Consignment Id</p>
      <div>
        <span class="consignment-id">{{ order.id }}</span>
        <img class="consignment-img" src="../assets/resource/ic_copy.svg" />
      </div>
    </div>
    <div class="shipping">
      <p class="shipping-title w-1/4">Shipping Info</p>
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
      <div class="timeline-img">
        <div class="status">
          <img src="../assets/resource/shipped.svg" class="box" />
          <p class="text">Confirm</p>
        </div>
        <div class="status">
          <img src="../assets/resource/truck.svg" class="box" />
          <p class="text">Picked-up</p>
        </div>
        <div class="status">
          <img src="../assets/resource/shipped.svg" class="box" />
          <p class="text">In Transit</p>
        </div>
        <div class="status">
          <img src="../assets/resource/truck.svg" class="box" />
          <p class="text">Out for Delivery</p>
        </div>
        <div class="status">
          <img src="../assets/resource/shipped.svg" class="box" />
          <p class="text">Return</p>
        </div>
      </div>
      <div class="timeline-details">
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
    <div class="product">
      <div class="w-1/2">
        <p class="product-title">Product Description</p>
        <div class="product-list">
          <p class="product-list-item">01 Black Tshirt</p>
          <p class="product-list-item">02 Knee Guard</p>
        </div>
      </div>
      <div class="w-1/2">
        <div class="receipt">
          <p class="receipt-title">Receipt</p>
          <button class="receipt-cash">
            <img src="../assets/resource/ic_cash.svg" class="receipt-cash-icon" />
            Cash On Delivery
          </button>
        </div>
        <div class="receipt-details">
          <div class="element">
            <p class="element-name">Product price</p>
            <p>&#2547; 700</p>
          </div>
          <div class="element">
            <p class="element-name">Delivery Charge</p>
            <p>&#2547; 60</p>
          </div>
          <p class="element dotted-separator"></p>
          <div class="element">
            <p class="total">Total</p>
            <p class="total-price">&#2547; 760</p>
          </div>
        </div>
      </div>
    </div>
    <div class="merchant">
      <p class="merchant-title">Seller Info</p>
      <div class="merchant-info">
        <img src="../assets/resource/logo.png" class="merchant-logo" />
        <div>
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
