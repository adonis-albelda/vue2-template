<template>
  <div>
    <table>
      <tr>
        <td>Shipping Fee</td>
        <td>{{shippingFee}}</td>
        <td>
          <button @click="shippingFee = Math.floor(Math.random() * (10 - 1 + 1)) + 1">Change Shipping Fee</button>
        </td>
      </tr>
      <tr>
        <td>Extra Fee</td>
        <td>{{extraFee}}</td>
        <td>
          <button @click="extraFee = Math.floor(Math.random() * (10 - 1 + 1)) + 1">Change Extra Fee</button>
        </td>
      </tr>
      <tr>
        <td>Total Orders</td>
        <td>{{totalOrders}}</td>
        <td>
          <button>Change Total Orders</button>
        </td>
      </tr>
      <tr>
        <td>Quantity</td>
        <td>{{quantity}}</td>
        <td>
          <button>Change Quantity</button>
        </td>
      </tr>
      <tr>
        <td>Total</td>
        <td>{{total}}</td>
      </tr>
    </table>
    <!-- <h1>The sum of first number and second number is : {{ total  }}</h1>
    <button @click="changeFirstNumber">Update first number</button> -->
    <!-- <header class="main-header">
      <h1 @click="changeFirstName">{{ firstName }}</h1>
      <p>
        {{todos}}
      </p>
    </header>
    <button @click="changeTodosAvailability">Set todos as Available</button>
    <button @click="changeTodos">Set todos as Available</button>
    <button @click="changeFirstName">Set todos as Available</button>
    <button @click="changeLastName">Set todos as Available</button>
    <button @click="changeTodosAvailability">Set todos as Available</button>
    <button @click="changeTodosAvailability">Set todos as Available</button> -->
    <!-- <button @click="getTodos">Get Todos</button> -->
    <!-- <footer class="main-footer">this is footer</footer> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      shippingFee:0,
      totalOrders:0,
      extraFee:0,
      quantity:0,
      date:null
      // total:0
      // title:'This is DX'
    };
  },
  created() {
    // this.changeFirstName()
    // this.getTodos()
    // this.title = 'dsddasdasdddsa'
  },
  mounted() {
    // this.totalValue()
  },
  methods: {
    // changeShippingFee() {
    //   this.shippingFee = Math.floor(Math.random() * (10 - 1 + 1)) + 1;
    //   this.getCartTotal()
    // },
    // changeExtraFee() {
    //   this.extraFee = Math.floor(Math.random() * (10 - 1 + 1)) + 1;
    //   this.getCartTotal()
    // },
    // changeDate() {
    //   this.date = new Date()
    //   this.getCartTotal()
    // },
    // changeFirstNumber() {
    //   this.firstNumber = 10
    //   this.discount 
    //   this.totalValue()
    // },
    // getCartTotal() {
    //   let discount = 0
    //   let totalValueOfOrders = 20
    //   let isDateValid = true
      
    //   if (totalValueOfOrders > 5000 && isDateValid) {
    //     discount = 20
    //   }

    //   this.total = (this.shippingFee + this.extraFee + (this.totalOrders * this.quantity)) - discount
    // },
    // changeTodosAvailability() {
    //   this.isTodosAvailable = !this.isTodosAvailable;
    // },
    // totalValue() {
    //   this.total = this.firstNumber + this.secondNumber
    // },  
    // changeTodos() {
    //   /** extra codes */
    //   this.isTodosAvailable = !this.isTodosAvailable;
    // },
    // changeFirstName() {
    //   /** extra codes */
    //   this.isTodosAvailable = !this.isTodosAvailable;
    // },
    // changeLastName() {
    //   /** extra codes */
    //   this.isTodosAvailable = !this.isTodosAvailable;
    // },
    // getTodos() {
    //   fetch("https://jsonplaceholder.typicode.com/todos")
    //     .then((response) => response.json())
    //     .then((json) => {
    //       this.todos = json;
    //       console.table(this.todos);
    //     });
    // },
  },
  computed: {
    // title() {
    //   return "This is DX Form"
    // },
    total() {
      // computation for discount
      // let discount = 0
      // let totalValueOfOrders = 20
      // let isDateValid = true
      
      // if (totalValueOfOrders > 5000 && isDateValid) {
      //   discount = 20
      // }

      // return (this.shippingFee + this.extraFee + (this.totalOrders * this.quantity)) - discount
    }
  },
  watch: {
    // isTodosAvailable(newVal) {
    //   if (newVal) {
    //     this.getTodos();
    //   }
    // },
  },
};
</script>

<style scoped>
.main-footer {
  width: 100%;
  height: 100px;
  background-color: blue;
}
</style>

<style scoped>
.main-header {
  width: 100%;
  height: 100px;
  /* background-color: red; */
}
</style>
