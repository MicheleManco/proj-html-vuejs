<template>
  <div id="bg-dark-blue">
    <div id="centratore-top">
      <div id="superiore">

        <div id="col-1">
          <img src="../assets/logo-light.png" alt="">
          <p>Start working with Landrick that can provide everything you need to generate awereness drive traffic, connect.</p>
          <div id="socials">
            <div>icona</div>
            <div>icona</div>
            <div>icona</div>
            <div>icona</div>
          </div>
        </div>

        <div id="col-2">
          <h3 class="section-ft">Company</h3>
          <ul>
            <li v-for="link,i in companyLinks" :key="i"><a class="link-decoration" href="">{{link.text}}</a></li>
          </ul>
        </div>

         <div id="col-3">
          <h3 class="section-ft">Usefull Links</h3>
          <ul>
            <li v-for="link,i in usefullLinks" :key="i"><a class="link-decoration" href="">{{link.text}}</a></li>
          </ul>
        </div>

        <div id="col-4">
          <h3 class="section-ft">Newsletter</h3>
          <p>Sign up and receive the latest tips via email</p>
          <div>Write your email*</div>
          <div id="user-email">icona Your email:</div>
          <div id="btn-sub">Subsribe</div>
        </div>

        
      </div>
    </div>
    <div id="divisorio">
      <div id="centratore-bottom">
        <div id="inferiore">
          <div>2020 Landrick. Design with love by Shreethemes.</div>

          <div id="credit-cards">
            <div class="card"><img src="../assets/american-ex.png" alt=""></div>
            <div class="card"><img src="../assets/discover.png" alt=""></div>
            <div class="card"><img src="../assets/master-card.png" alt=""></div>
            <div class="card"><img src="../assets/paypal.png" alt=""></div>
            <div class="card"><img src="../assets/visa.png" alt=""></div>
          </div>
        </div>
      </div>
    </div>
    
    
  </div>
</template>

<script>
export default {
  name: 'MyFooter',
  data() {
    return {
      companyLinks:[
      {
        text: "About us"
      },
      {
        text:"Services"
      },
      {
        text:"Team"
      },
      {
        text:"Pricing"
      },
      {
        text:"Project"
      },
      {
        text:"Careers"
      },
      {
        text:"Blog"
      },
      {
        text:"Login"
      }
    ],
    usefullLinks:[
      {
        text:"Terms of Services"
      },
       {
        text:"Privacy Policy"
      },
       {
        text:"Documentation"
      },
       {
        text:"Changelog"
      },
       {
        text:"Components"
      },
    ]
  }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#btn-sub{
  color: #2f55d4;
  border: 1px solid #2f55d4;
  border-radius: 10px;
  padding: 10px;
  display: flex;
  justify-content: center;
}
#user-email{
  background-color: #27314f;
  padding: 10px;
  border-radius: 10px;
  margin: 10px 0;
}
.link-decoration{
  text-decoration: none;
  color:#adb5bd;
}
li{
  line-height: 30px;
  list-style: none;
}
#bg-dark-blue{
  background-color: #202942;
  color:#adb5bd;
}
#centratore-top{
  width: 70%;
  margin: 0 auto;
}
#superiore{
  display: flex;
  justify-content: space-between;
}
#col-1{
width: 20%;
margin: 40px 0;
img{
  max-width: 100%;
  height: 30px;
  margin-bottom: 30px;
}
p{
  line-height: 25px;
  margin-bottom: 20px;
}
}
#col-2{
margin: 40px 0;
}
#col-3{
margin: 40px 0;
}
#col-4{
margin: 40px 0;
width: 20%;
p{
  line-height: 25px;
  margin-bottom: 20px;
}
}
.section-ft{
  color: white;
  margin-bottom: 30px;
}
#socials{
  display: flex;
}
#divisorio{
  border-top: 1px solid #adb5bd;
}
#centratore-bottom{
  width: 70%;
  margin: 0 auto;
}
#inferiore{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 0 ;
}
#credit-cards{
  display: flex;
  .card{
    margin-right: 5px;
    height: 30px;
    img{
      max-height: 100%;
    }
  }
}
</style>