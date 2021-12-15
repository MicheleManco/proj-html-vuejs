<template>
  <div class="container">
        <h2>Our rates for developer from landrick team</h2>
        <p class="text-gray">Start working with <span class="blue-text">Landrick</span> that can provide everything you neeed to generate awerness, drive traffic, connect.</p>
    <div class="bar">
      <div class="text-gray email"> Email Adress</div>
      <div class="btn-blue">Get Started</div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'SectionCinque',
}
</script>


<style scoped lang="scss">
p{
  line-height: 25px;
  margin: 35px 0;
}
.email{
  margin-left: 20px;
}
.text-gray{
color: #8492a6;
}
.container{
  width: 40%;
  margin: 80px auto;
  text-align: center;
  .bar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    border: 1px solid  #adb5bd;
    border-radius: 20px;
    height: 40px;
    padding: 2px;
    .btn-blue{
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: #2f55d4;
      width: 130px;
      border-radius: 20px;
      color: white;
      height: 100%;
    }
  }
}
</style>