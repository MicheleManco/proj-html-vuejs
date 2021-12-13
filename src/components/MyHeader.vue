<template>
  <div>
    <div id="centratore">
      <div id="logo"><img src="../assets/logo-dark.png" alt=""></div>
      <nav>
        <ul>
          <li><a href="">HOME</a></li>
          <li><a href="">LANDING</a></li>
          <li><a href="">PAGES</a></li>
          <li><a href="">DOCS</a></li>
        </ul>
      </nav>
      <div class="ricerca btn-account">
        <div>icona</div>
        <div class="btn-light">pulasnte1</div>
        <div class="btn-light">>pulasnte2</div>
        <div class="btn-light">>pulasnte3</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyHeader',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#centratore{
  width: 70%;
  margin: 20px auto;
  display: flex;
  justify-content: space-between;
  #logo{
    width: 20%;
    img{
      max-width: 100%;
      height: 35px;
    }
  }
  ul{
    display: flex;
    list-style: none;
    li{
      margin-right: 35px;
    }
    a{
      color: black;
      text-decoration: none;
    }
  }
  .ricerca{
    display: flex;
    .btn-light{
      height: 35px;
      width: 35px;
      margin: 0 5px;
      background-color: #2f55d41a;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  }
}
</style>
