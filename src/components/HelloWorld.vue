<template>
  <div class="hello">
    <nav>
      <ul>
        <h1>Growpartner Coffee Shop</h1>
      </ul>
    </nav>
    <div class="container-fluid">
      <div class="content-left col-xs-3">
        <h3>Stock Available</h3>
        <ol>
          <h4 class="col-xs-6">Water</h4>
          <h4 class="col-xs-6">1000</h4>
          <h4 class="col-xs-6">Milk</h4>
          <h4 class="col-xs-6">1000</h4>
          <h4 class="col-xs-6">Tea</h4>
          <h4 class="col-xs-6">200</h4>
          <h4 class="col-xs-6">Coffee</h4>
          <h4 class="col-xs-6">200</h4>
          <h4 class="col-xs-6">Sugar</h4>
          <h4 class="col-xs-6">500</h4>
        </ol>
        <div class="d-grid col-6 mx-auto">
          <button class="btn">Refill Stock</button>
        </div>
      </div>
      <div class="content-right col-xs-9">
        <h2>Welcome to the Coffee Shop</h2>
        <h3>Select order Preferences</h3>

        <div class="mb-3 row-xs-6">
          <select class="form-select" required aria-label="select example">
            <option value=""><h6>Selet Drink Type</h6></option>
            <option value="1">Strong Coffee</option>
            <option value="2">Light Coffee</option>
            <option value="3">Strong Tea</option>
            <option value="4">Light Tea</option>
          </select>
          <!-- <div class="invalid-feedback">Example invalid select feedback</div> -->
        </div>
        <div class="mb-4 row-xs-6">
          <select class="form-select" required aria-label="select example">
            <option value="">Enter No of Cups</option>
            <option value="1">
              Strong Coffee ( Rs. 100 ): milk 10 coffee 8 water 4 tea 0
            </option>
            <option value="2">
              Light Coffee ( Rs. 75 ): milk 15 coffee 4 water 4 tea 0
            </option>
            <option value="3">
              Strong Tea ( Rs. 60 ): milk 10 coffee 0 water 8 tea 8
            </option>
            <option value="4">
              Light Tea ( Rs. 50 ): milk 15 coffee 0 water
            </option>
          </select>
          <!-- <div class="invalid-feedback">Example invalid select feedback</div> -->
        </div>

        <div class="form-check">
          <input
            class="form-check-input"
            type="checkbox"
            value=""
            id="flexCheckChecked"
            checked
          />
          <label class="form-check-label" for="flexCheckChecked">
            <h5>With Sugar</h5>
          </label>
        </div>
        <div class="d-grid col-6 mx-auto">
          <button class="btn">Pay Rs. 0</button>
        </div>
        
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    drawer: false,
    group: null,
  }),
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul {
  flex-direction: column;
  text-align: left;
  padding: 12px;
  background: black;
  color: white;
}

h3 {
  justify-content: left;
  color: black;
  /* text-align: left; */
  padding-left: 0px;
  padding-bottom: 30px;
  padding-top: 5%;
}
h2 {
  justify-content: right;
  color: black;
  padding-top: 70px;
  padding-right: 20px;
}
h1 {
  padding-left: 20px;
}
h4 {
  color: black;
}
h5 {
  color: black;
  padding-left: 10px;
}
h6 {
  color: black;

  font-size: 21px;
}
.content-left {
  background: rgb(236, 213, 182);
  padding-top: 10px;
  padding-bottom: 33%;
  margin-left: -12px;
}
.mb-3 {
  padding: 15px;
  color: gray;
  text-align-last: center;
  font-size: 15px;
  
}
.mb-4 {
  color: gray;
  text-align-last: center;
  font-size: 15px;
  padding: 15px;
}
.btn {
  background: rgb(68, 35, 35);
  font-size: 18px;
  padding-left: 10%;
  padding-right: 10%;
  margin-top: 5%;
}
.form-select {
  margin-top: 20px;
}
.form-check {
  margin-top: 40px;
}
.dropdown-toggle {
  color: black;
}
</style>
