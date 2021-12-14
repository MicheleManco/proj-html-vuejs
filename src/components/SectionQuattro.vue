<template>
  <div class="centratore">
    <div id="sopra">
        <h2>Our rates for developer from landrick team</h2>
        <p>Start working with <span class="blue-text">Landrick</span> that can provide everything you neeed to generate awerness, drive traffic, connect.</p>
    </div>
    <div id="row-plans">
          <div  v-for="plan,i in plans" :key="i" class="card">
              <div class="container">
                <div class="btn-light">{{plan.etichetta}}</div>
                <h1>{{plan.price}}</h1>
                <div class="text-gray">Per month</div>
                <p class="text-gray">{{plan.text}}</p>
                <hr>
                <ul>
                  <li class="text-gray " v-for="vantaggio,i in plan.vantaggi" :key="i"><i class="far fa-check-circle"></i>{{vantaggio}}</li>
                </ul>
              </div>
              <div class="btn-blue">Buy Now</div>
              <div class="text-gray">*No credit card required</div>
          </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'SectionQuattro',
  data() {
    return {
      plans:[
        {
          price:"$9.00",
          text:"All the basics for businesses that are just getting started.",
          etichetta:"Basic",
          vantaggi:[
            "Full Access","Enhached Security","Source Files","1 Domain Free","Enhaced Security"
          ]
        },
         {
          price:"$39.00",
          text:"Better for growing businesses that want more customers.",
          etichetta:"Business",
          vantaggi:[
            "Full Access","Enhached Security","Source Files","1 Domain Free","Enhaced Security"
          ]
        },
         {
          price:"$79.00",
          text:"Advanced features for pros who need mor customization.",
          etichetta:"Enterprise",
          vantaggi:[
            "Full Access","Enhached Security","Source Files","1 Domain Free","Enhaced Security"
          ]
        },
      ]
    }}
}
</script>


<style scoped lang="scss">
li{
  list-style: none;
}
h1{
  margin-bottom: 10px;
}
#row-plans{
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  .card{
    width: 25%;
    border: 1px solid  #adb5bd;
    box-shadow: 0 3px #adb5bd;
    border-radius: 10px;
    padding: 30px;
  }
}
.fa-check-circle{
  color: #2f55d4;
  margin-right: 5px;
}

.text-gray{
  color: #8492a6;
  margin: 15px 0;
}
.btn-light{
  background-color: #2f55d41a;
  border-radius: 20px;
  width: 100px;
  padding: 5px;
  margin-bottom: 25px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #2f55d4;
  border: 1px solid #adb5bd;
}
.btn-blue{
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #2f55d4;
  color: white;
  margin-top: 25px;
  margin-right: 10px;
  padding: 8px 20px 8px;
  border-radius: 7px;
  width: 100%;
}
.centratore{
  width: 70%;
  margin: 100px auto;
  #sopra{
    text-align: center;
    width: 40%;
    margin: 0 auto;
    p{
      color: #8492a6;
      line-height: 25px;
      margin-top: 30px;
      span{
        color: #2f55d4;
      }
    }
  }
}
</style>