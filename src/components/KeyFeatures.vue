<template>
  <div id="centratore">
      <div id="title">
        <h2>Key Features</h2>
        <p>Start working with <span>Landrick</span> Landrick that can provide everything you need to generate awareness, drive traffic, connect. </p>
      </div>
      <div id="row-features">
          <div  v-for="feature,i in features" :key="i" class="card">
              <div class="container">
                <div class="icona-features"><i :class="feature.icon"></i></div>
                <h3>{{feature.title}}</h3>
                <p>{{feature.text}}</p>
                <a href="">Read More <i class="fas fa-chevron-right"></i></a>
              </div>
              
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'KeyFeatures',
   data() {
    return {
      features:[
        {
          title:"Modular",
          text:"Composed in a pseudo-latin language which more or less corresponds",
          icon:"fas fa-layer-group"
        },
        {
          title:"Responsive",
          text:"Composed in a pseudo-latin language which more or less corresponds",
          icon:"fas fa-desktop"
        },
        {
          title:"Customizable",
          text:"Composed in a pseudo-latin language which more or less corresponds",
          icon:"fas fa-crosshairs"
        },
        {
          title:"Scalable",
          text:"Composed in a pseudo-latin language which more or less corresponds",
          icon:"fas fa-expand-arrows-alt"
        }
      ]
    }}
}
</script>


<style scoped lang="scss">
.fa-chevron-right{
  font-size: 10px;
}
#centratore{
    width: 70%;
    margin: 50px auto;
    #title{
        width: 50%;
    }
    p{
        color: #8492a6;
        margin: 15px 0 30px 0;
        line-height: 25px;
        span{
            color: #2f55d4;
        }
    }
    #row-features{
        display: flex;
        justify-content: space-between;
        margin-top: 60px;
    }
    .card{
        width: 22%;
        border: 1px solid #e9ecef;
        .container{
            padding: 25px;
        }
        .icona-features{
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #2f55d41a;
            color: #2f55d4;
            width: 60px;
            height: 60px;
            margin-bottom: 20px;
            border-radius: 7px;
        }
        a{
            text-decoration: none;
            color: #2f55d4;
        }
    }
}
</style>