<template>
  <div class="container">
    <div class="row pt-3 pb-3">
      <div class="col-md-3">Logo</div>
      <div class="col-md-9 nav p-0">
        <router-link class="nav-link" to="/">Home</router-link>
        <router-link class="nav-link" to="/about">Themes</router-link>
        <router-link class="nav-link" to="/contacts">
          Topics <span> <i class="fa fa-angle-down"></i> </span>
          <div class="drop-down">
            <router-link class="nav-link-drop" to="/portfolio">Introduction To Shoppify <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Your Account <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Migrating To Shoppify <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Shoppify Community <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Selling Online <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Selling Inperson <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Products <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Location <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Themes For Your Online Store <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Payments <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Shopping <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Domain <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Orders <hr class="under"></router-link>
            <!-- <router-link class="nav-link-drop" to="/how_to">Online Checkout <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Taxes <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Customers <hr class="under"></router-link> -->
          </div>
        </router-link>
        <router-link class="nav-link" to="/portfolio">
          Support <span><i class="fa fa-angle-down"></i> </span>
          <div class="drop-down">
            <router-link class="nav-link-drop" to="/portfolio">Introduction To Shoppify <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Your Account <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Migrating To Shoppify <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Shoppify Community <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Selling Online <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Selling Inperson <hr class="under"></router-link>
            <router-link class="nav-link-drop" to="/how_to">Products <hr class="under"></router-link>
          </div>

        </router-link>
        <router-link class="nav-link" to="/how_to">Shoppify.com</router-link>
        <router-link class="nav-link" to="/how_to">Login</router-link>
        <router-link class="nav-link btn btn-success" to="/how_to">SignUp</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'nav',
  props: {}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .nav {
    display: flex;
    flex-direction: row;
  }
  .nav-link {
    flex: 1;
  }

  .drop-down {
    /* display: none; */
    position: absolute;
    /* display: flex; */
    flex-direction: column;
    background: whitesmoke;
    z-index: 1;
    /* width: 130px; */
    padding-left: 3px;
    top: 40px;
    border-radius: 5px;
    box-shadow: 5px 10px 10px black;
    transition-duration: 1s;
    overflow: hidden;
    height: 0;
    opacity: 0;
  }

  .nav-link-drop {
    display: inline-block;
    color: blue;
    text-decoration: none;
    padding-top: 5px;
    padding-bottom: 5px;
  }

  .nav-link:hover .drop-down {
    display: flex;
    height: auto;
    opacity: 1;
  }
  .under {
    background: blue;
    margin-top: 0;
    margin-bottom: 0;
    height: 1px;
    /* width: 80%; */
    position: relative;
    left: 0;
    width: 0;
    transition-duration: .5s;
  }
  .fa-angle-down {
    transition-duration: .5s;
  }

  .nav-link:hover .fa-angle-down {
    transform: rotate(180deg)
  }
  .nav-link-drop:hover .under {
    width: 100%;
  }

</style>
