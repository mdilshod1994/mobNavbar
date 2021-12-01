<template>
<div class="nav">
  <h1>
    We know CSS like our 5 finger!!!
  </h1>
  <div class="mob_nav">
    <ul>
      <li class="list active">
        <router-link to="">
          <span class="icon">
           <ion-icon name="home-outline"></ion-icon>
          </span>
          <span class="text">
            Home
          </span>
        </router-link>
      </li>
      <li class="list">
        <router-link to="">
          <span class="icon">
            <ion-icon name="person-circle-outline"></ion-icon>
          </span>
          <span class="text">
            Profile
          </span>
        </router-link>
      </li>
      <li class="list">
        <router-link to="">
          <span class="icon">
            <ion-icon name="mail-open-outline"></ion-icon>
          </span>
          <span class="text">
            Messages
          </span>
        </router-link>
      </li>
      <li class="list">
        <router-link to="">
          <span class="icon">
            <ion-icon name="folder-open-outline"></ion-icon>
          </span>
          <span class="text">
            About
          </span>
        </router-link>
      </li>
      <li class="list">
        <router-link to="">
          <span class="icon">
            <ion-icon name="call-outline"></ion-icon>
          </span>
          <span class="text">
            Contact
          </span>
        </router-link>
      </li>
      <div class="indicator"></div>
    </ul>
  </div>
</div>
  
</template>

<script>

export default {
  name: 'HelloWorld',
  data () {
    return {

    }
  },
  methods:{

  },
  mounted(){
    const list = document.querySelectorAll('.list')
    function activeLink() {
      list.forEach((item)=>
      item.classList.remove('active'))
      this.classList.add('active')
    }
    list.forEach((item)=>
      item.addEventListener('click', activeLink)
    )
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
