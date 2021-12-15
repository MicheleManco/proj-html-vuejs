<template>
  <div id="bg-dark-blue">
    <div id="centratore-top">
      <div id="superiore">

        <div id="col-1">
          <img src="../assets/logo-light.png" alt="">
          <p>Start working with Landrick that can provide everything you need to generate awereness drive traffic, connect.</p>
          <div id="socials">
            <div class="social-btn"><i class="fab fa-facebook-f"></i></div>
            <div class="social-btn"><i class="fab fa-instagram"></i></div>
            <div class="social-btn"><i class="fab fa-twitter"></i></div>
            <div class="social-btn"><i class="fab fa-linkedin-in"></i></div>
          </div>
        </div>

        <div id="col-2">
          <h3 class="section-ft">Company</h3>
          <ul>
            <li v-for="link,i in companyLinks" :key="i"><a class="link-decoration" href=""><i class="fas fa-chevron-right"></i>{{link.text}}</a></li>
          </ul>
        </div>

         <div id="col-3">
          <h3 class="section-ft">Usefull Links</h3>
          <ul>
            <li v-for="link,i in usefullLinks" :key="i"><a class="link-decoration" href=""><i class="fas fa-chevron-right"></i>{{link.text}}</a></li>
          </ul>
        </div>

        <div id="col-4">
          <h3 class="section-ft">Newsletter</h3>
          <p>Sign up and receive the latest tips via email</p>
          <div>Write your email*</div>
          <div id="user-email"><i class="far fa-envelope"></i>Your email:</div>
          <div id="btn-sub">Subsribe</div>
        </div>

        
      </div>
    </div>
    <div id="divisorio">
      <div id="centratore-bottom">
        <div id="inferiore">
          <div><i class="far fa-copyright"></i> 2020 Landrick. Design with <i class="fas fa-heart"></i> by Shreethemes.</div>

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
.fa-heart{
  color: #e43f52;
}
.social-btn{
  height: 30px;
  width: 30px;
  border: 1px solid white;
  border-radius: 5px;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-right: 7px;
}
.fa-envelope{
  margin: 0 10px;
}
.fa-chevron-right{
  margin-right: 10px;
  font-size: 10px;
}
#btn-sub{
  color: #2f55d4;
  border: 1px solid #2f55d4;
  border-radius: 10px;
  padding: 10px;
  display: flex;
  justify-content: center;
  margin-top: 20px;
}
#user-email{
  background-color: #27314f;
  padding: 10px;
  border-radius: 10px;
  margin-top: 15px;
}
.link-decoration{
  text-decoration: none;
  color:#adb5bd;
}
li{
  line-height: 35px;
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