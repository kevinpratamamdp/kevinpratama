<template>
  <div>
    <ul>
      <h1>Login</h1>
      <li>
        <form>
          <div class="mb-3">
              <label for="exampleInputEmail1" class="form-label">Email address</label>
              <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
              <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
          </div>
          <div class="mb-3">
              <label for="exampleInputPassword1" class="form-label">Password</label>
              <input type="password" class="form-control" id="exampleInputPassword1">
          </div>
          <div class="mb-3 form-check">
              <input type="checkbox" class="form-check-input" id="exampleCheck1">
              <label class="form-check-label" for="exampleCheck1">Check me out</label>
          </div>
          <router-link to="/dashboard" class="w-100 btn btn-lg btn-primary" type="submit">Sign in</router-link>   
          <router-link :to="{name: 'register'}" class="w-100 btn btn-lg btn-secondary mt-1" type="button">Register</router-link>

          <router-link :to="{path: '/'}">Back To Home</router-link>
          
        </form>
      </li>
    </ul>    
  </div>    
</template>
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 20px 10px;
}
</style>