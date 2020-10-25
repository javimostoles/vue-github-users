<template>

  <div class="vue-template">
    <form class="inner-block">
      <h3>Sign In</h3>
      <div class="form-group">
          <label>Email address</label>
          <input type="email" class="form-control form-control-lg" />
      </div>
      <div class="form-group">
          <label>Password</label>
          <input type="password" class="form-control form-control-lg" />
      </div>
      <button type="submit" class="btn">Sign In</button>
      <p class="forgot-password">
          <router-link to="/forgot-password">Forgot password ?</router-link>
      </p>
  </form>
  </div>

</template>

<style lang="scss">

.vue-template{
  display: flex;
  justify-content: center;
  align-items: center;
}
.navbar-light {
  background-color: #ffffff;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
}



.inner-block {
  width: 450px;
  margin: auto;
  background: #ffffff;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
  padding: 40px 55px 45px 55px;
  border-radius: 15px;
  transition: all .3s;
}



.vertical-center .form-control:focus {
  border-color: #2554FF;
  box-shadow: none;
}

.vertical-center h3 {
  text-align: center;
  margin: 0;
  line-height: 1;
  padding-bottom: 20px;
}

label {
  font-weight: 500;
}

.vertical-center {
  display: flex;
  text-align: left;
  justify-content: center;
  flex-direction: column;    
}

.inner-block {
  width: 450px;
  margin: auto;
  background: #ffffff;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
  padding: 40px 55px 45px 55px;
  border-radius: 15px;
  transition: all .3s;
  .btn{
    font-size: 0.75rem;
    height: 2.5rem;
    line-height: 2.5rem;
    padding: 0 1.5rem;
    color: white;
    background: #8E49E8;
    text-transform: uppercase;
    border-radius: .25rem;
    letter-spacing: .2em;
    transition: background .2s;
    border:0;
    display: flex;
    justify-content: flex-start;
  }
 
}

.form-group{
  display: flex;
  flex-direction: column;
  margin: 1em 0;
   label {
    font-weight: 500;
    display:flex;
    justify-content: flex-start;
  }
  input {
    margin: .5em 0;
    padding: .5em;
    border-radius: 5px;
    border: 1px solid grey;
  }

}


.forgot-password,
.forgot-password a {
  text-align: right;
  font-size: 13px;
  padding-top: 10px;
  color: #7a7a7a;
  margin: 0;
}

.forgot-password a {
  color: #2554FF;
}

</style>