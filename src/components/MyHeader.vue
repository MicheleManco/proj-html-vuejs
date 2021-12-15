<template>
  <div>
    <div id="centratore">
      <div id="logo"><img src="../assets/logo-dark.png" alt=""></div>
      <nav>
        <ul>
          <li v-for="link,i in linkNav" :key="i" :class="link.active ? 'active':''"><a href="">{{link.text}}<span class="tendina"><i class="fas fa-chevron-down"></i></span></a></li>
        </ul>
      </nav>
      <div class="ricerca btn-account">
        <div id="lente"><i class="fas fa-search"></i></div>
        <div class="btn-light"><i class="fab fa-github"></i></div>
        <div class="btn-light"><i class="fab fa-stack-overflow"></i></div>
        <div class="btn-light"><i class="far fa-user"></i></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyHeader',
  data() {
    return {
      linkNav:[
        {
          text:"HOME",
          active:false
        },
        {
          text:"LANDING",
          active:true
        },
        {
          text:"PAGES",
          active:false
        },
        {
          text:"DOCS",
          active:false
        },
      ]
    }}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#centratore{
  width: 70%;
  margin: 0px auto;
  padding: 20px 0;
  display: flex;
  justify-content: space-between;
  #logo{
    width: 20%;
    img{
      max-width: 100%;
      height: 35px;
    }
  }
nav{
  display: flex;
  align-items: center;
}
  ul{
    display: flex;
    list-style: none;
    li{
      margin-right: 40px;
    }
    .active{
        a{
          color: #2f55d4;
        }
      }
    a{
      color: black;
      text-decoration: none;
    }
    .tendina{
      margin-left: 5px;
    }
  }
  .ricerca{
    display: flex;
    #lente{
      color: #8492a6;
      display: flex;
      align-items: center;
      .fa-search{
        font-size: 18px;
        margin-right: 5px;
      }
    }
    .btn-light{
      height: 35px;
      width: 35px;
      margin: 0 5px;
      background-color: #2f55d41a;
      display: flex;
      justify-content: center;
      align-items: center;
      border-radius: 5px;
      color: #2f55d4;
    }
    .btn-light:hover{
        color: white;
        background-color: #2f55d4;
    }
  }
}

</style>
