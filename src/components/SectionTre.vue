<template>
  <div>
    <div class="centratore">
      <div id="description">
          <h1>Build tools and extensive documentation</h1>
          <p>You can combine all the Landrick templates into a single one, you can take a component from the Application theme and use it in the Website</p>
          <div class="text"><span><i class="far fa-check-circle"></i></span>Digitial Marketing Solutions for Tomorrow</div>
          <div class="text"><span><i class="far fa-check-circle"></i></span>Our Talented &amp; Experienced Marketing Agency</div>
          <div class="text"><span><i class="far fa-check-circle"></i></span>Create your own skin to match your brand</div>
          <div class="btn">Get started <i class="fas fa-arrow-right"></i></div>      
      </div>

      <div><img src="../assets/1.png" alt=""></div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'SectionTre',
}
</script>


<style scoped lang="scss">
.text{
  color: #8492a6;
  line-height: 30px;
  span{
    color: #2f55d4;
    margin-right: 5px;
  }
}
p{
  color: #8492a6;
  line-height: 25px;
  margin: 30px 0;
}
.centratore{
    width: 70%;
    margin: 70px auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    #description{
      width: 48%;
    }
    img{
      height: 400px;
    }
    .btn{
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #2f55d4;
      color: white;
      margin-top: 25px;
      margin-right: 10px;
      padding: 8px 20px 8px;
      border-radius: 7px;
      width: 30%;
      .fa-arrow-right{
        font-size: 10px;
        margin-left: 7px;
      }
    }
}
</style>