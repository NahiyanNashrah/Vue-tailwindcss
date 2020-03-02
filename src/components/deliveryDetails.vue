<template>
  <div>
    <div class="container md:w-8/12 mt-1">
      <div class="bg-white shadow-gray px-4 py-4 flex mt-1">
        <div class="w-1/2">
          <h1 class="text-gray-500">Consignment Id</h1>
        </div>
        <div class="w-1/2 flex flex-col items-end">
          <h2 class="text-black font-bold">{{order.id}}</h2>
        </div>
      </div>
      <div class="bg-white shadow-gray px-4 py-4 mt-1 flex flex-row justify-between">
        <div class="w-1/4">
          <h1 class="text-gray-500">Shipping Info</h1>
        </div>
        <div class="w-1/2 flex flex-col items-end">
          <h2 class="text-black font-bold">{{ user.phone }}</h2>
          <p>{{ user.name }}</p>
          <p>{{ user.address }}</p>
        </div>
      </div>

      <div class="bg-white shadow-gray py-4 px-4 mt-1 flex flex-col">
        <h1 class="text-black font-bold mb-2">Timeline</h1>
        <div class="flex flex-row">
          <hr class="w-1 h-12 bg-red-500 rounded mr-2" />
          <div class="mb-2">
            <h3 class="font-medium">Your order has been picked-up!</h3>
            <p class="text-gray-400">March 1,2020,10:00</p>
          </div>
        </div>
        <div class="flex flex-row">
          <hr class="w-1 h-12 bg-blue-500 rounded mr-2" />
          <div class="mb-2">
            <h3 class="font-medium">Our delivery man is on his way to pick up your order.</h3>
            <p class="text-gray-400">March 1,2020,10:00</p>
          </div>
        </div>
        <div class="flex flex-row">
          <hr class="w-1 h-12 bg-green-500 rounded mr-2" />
          <div class="mb-2">
            <h3 class="font-medium">Your Order has been confirmed!</h3>
            <p class="text-gray-400">March 1,2020,10:00</p>
          </div>
        </div>
      </div>
      <div class="bg-white shadow-gray py-4 px-4 mt-1 flex flex-row">
        <div class="w-1/2">
          <h1 class="text-black font-bold">Product Description</h1>
          <div class="flex flex-col items-start font-normal mt-2">
            <p>01 Black Tshirt</p>
            <p>02 Knee Guard</p>
          </div>
        </div>
        <div class="w-1/2">
          <h1 class="text-black font-bold">Receipt</h1>
          <div class="w-full flex flex-col mt-2">
            <div class="flex font-normal mb-2">
              <p class="w-1/2 md:w-2/3 flex flex-col items-start">Product price</p>
              <p class="w-1/2 md:w-1/3 flex flex-col items-end">&#2547; 700</p>
            </div>
            <div class="w-full flex font-normal mb-2">
              <p class="w-1/2 flex flex-col items-start">Delivery Charge</p>
              <p class="w-1/2 flex flex-col items-end">&#2547; 60</p>
            </div>
            <hr />
            <div class="w-full flex font-medium mb-2">
              <p class="w-1/2 flex flex-col items-start">Total</p>
              <p class="w-1/2 flex flex-col items-end">&#2547; 760</p>
            </div>
          </div>
        </div>
      </div>

      <div class="bg-white shadow-gray py-4 px-4 mt-1">
        <h1 class="text-black font-bold">Seller Info</h1>
        <div class="flex flex-row">
          <div class="w-20">
            <img src="../assets/resource/logo.png" class="object-cover h-20" />
          </div>
          <div class="w-6/9">
            <h2 class="capitalize text-red-500">Abibas apparels joy endless</h2>
            <p class="capitalize text-black">Tshirt,panjabi,Men's wear</p>
          </div>
        </div>
      </div>
      <div class="bg-white shadow-gray py-4 px-4 mt-1">
        <div class="flex flex-row">
          <button
            class="w-1/2 bg-red-600 hover:bg-red-700 text-white uppercase font-bold py-2 px-2 mr-3 rounded"
          >Call Support</button>
          <button
            class="w-1/2 bg-gray-500 hover:bg-gray-700 text-black uppercase font-bold py-2 px-2 rounded"
          >Chat Bot</button>
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
      }
    };
  }
};
</script>
<style src="../assets/style/main.css">
</style>