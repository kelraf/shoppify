<template>
  <div class="home">
    
    <Bunner />
    
    <div class="container">

      <div class="row ">
        <div class="col-12 pt-4">
           <h2 class="text-center"> Welcome to Shopify </h2>
        </div>
      </div>

      <WelcomeSectionOne />

      <!-- <WaysToSell /> -->

    </div>

  </div>
</template>

<script>
import Bunner from '../components/Bunner'
import WelcomeSectionOne from '../components/WelcomeSectionOne'
export default {
  name: 'home',
  components: {
    Bunner,
    WelcomeSectionOne
  }
}
</script>
