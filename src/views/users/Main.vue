<template>
  <div>
    <layout-main>
      <div class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
          <h1 class="h2">Users</h1>
      </div>
      <div class="row">
        <div v-for="user in datausers" :key="user" class="card col-md-3 mx-2 my-1">
            <img src="/PeopleIcon.png" class="card-img-top" alt="...">
            <div class="card-body">
                <h5 class="card-title">{{user.name}}</h5>
                <br/><hr/>
                <p class="card-text">
                    <center>Company</center>
                    {{user.company.name}}
                </p>
                <router-link :to="{name:'detailuser', 
                    params: { id: user.id, username: user.username }}" 
                    class="btn btn-primary">Detail User
                </router-link>
            </div>
        </div>
      </div>
    </layout-main>
  </div>
</template>

<script>
import LayoutMain from "@/views/LayoutMain"
export default {
    components: {
        LayoutMain
    },
    data(){
        return{
            datausers: null,
        }
    },
    methods: {
        loadUsers(){
            fetch("https://jsonplaceholder.typicode.com/users")
                .then(response => response.json()) // Then First,set response sebagai json
                .then(json => {
                    this.datausers = json;
                    console.log(json)
                })
                .catch(error => {
                    console.log(error);
                })
        }
    },
    mounted(){
        this.loadUsers();
        console.log(this.datausers)
    }
}
</script>