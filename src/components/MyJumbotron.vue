<template>
  <div>
    <div class="centratore">
      <div>
          <div class="btn-topic">Development</div>
          <h1>A Complete Developer Toolset</h1>
          <p>Launch your campaign and benefit from our expertise on designing and managing conversion centered bootstrap4 html page.</p>
          <div id="row-btns">
              <div class="btn blu">Get started</div>
              <div class="btn white">Documentation</div>
          </div>
          <div id="version">
              Current Version: v2.6.0
          </div>
      </div>

      <div><img src="../assets/about.png" alt=""></div>
    </div>
    <div><hr></div>
    <div class="centratore-sotto">
      <div id="brands">
        <div><img src="../assets/amazon.svg" alt=""></div>
        <div><img src="../assets/google.svg" alt=""></div>
        <div><img src="../assets/lenovo.svg" alt=""></div>
        <div><img src="../assets/paypal.svg" alt=""></div>
        <div><img src="../assets/shopify.svg" alt=""></div>
        <div><img src="../assets/spotify.svg" alt=""></div>
      </div>
    </div>
      
    
  </div>
</template>

<script>
export default {
  name: 'MyJumbotron',
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


<style scoped lang="scss">
hr{
  color: #e9ecef;
}
.centratore-sotto{
    width: 70%;
    margin: 0px auto;
    display: flex;
    align-items: center;
    #brands{
      margin: 30px 0;
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: 100%;
      height: 70px;
      div{
        display: flex;
        justify-content: center;
        width: 100px;
        img{
          width: 85%;
          max-height: 100%;
          color: #8492a6;
        }
      }
    }
}
.centratore{
    width: 70%;
    margin: 70px auto;
    display: flex;
    align-items: center;
    .btn-topic{
        background-color: #2f55d41a;
        padding:2px;
        color: #2f55d4;
        width: 95px;
        border-radius: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 13px;
    }
    h1{
        width: 50%;
        line-height: 50px;
        margin-top: 5px;
        margin-bottom: 15px;
    }
    p{
        color: #8492a6;
    }
    #row-btns{
        display: flex;
        align-items: center;
        margin: 20px 0 5px 0;
        .blu{
            display: flex;
            justify-content: center;
            background-color: #2f55d4;
            color: white;
            margin-right: 10px;
            padding: 8px 20px 8px;
            border-radius: 7px;
        }
        .white{
            color: #2f55d4;
            border: 1px solid #2f55d4;
            padding: 8px 20px 8px;
            border-radius: 7px;
        }
    }
    #version{
        color: #8492a6;
    }
}


</style>