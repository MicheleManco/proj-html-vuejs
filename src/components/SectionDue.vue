<template>
  <div id="centratore">
    <div id="sopra">
        <div class="blue-text">Quickstart</div>
        <h2>Awesome isn't it? Let's dive in!</h2>
        <p>Start working with <span class="blue-text">Landrick</span> that can provide everything you neeed to generate awerness, drive traffic, connect.</p>
    </div>
    
    <div id="container-riga">
        <div id="riga">
            <div class="btn active">npm</div>
            <div class="btn">nuget</div>
            <div class="btn">spm</div>
            <div class="btn">github</div>
        </div>
        <div><span><i class="fas fa-dollar-sign"></i></span> npm install <span>-g</span>claps.js</div>
    </div>

    <span class="checks"><i class="far fa-check-circle"></i> Organize your data</span>
    <span class="checks"><i class="far fa-check-circle"></i>  Work with any team</span>
  </div>
</template>

<script>

export default {
  name: 'SectionDue',
}
</script>


<style scoped lang="scss">
p{
    color: #8492a6;
}
.checks{
    margin-right: 25px;
    color: #8492a6;;
    .fa-check-circle{
        color: #2eca8b;
    }
}
h2{
    margin: 10px 0 25px 0;
}
.blue-text{
    color: #2f55d4;
}
#centratore{
    width: 40%;
    margin: 90px auto;
    #sopra{
        text-align: center;
        margin-bottom: 40px;
    }
    #container-riga{
        background-color: #202942;
        border-radius: 8px;
        padding: 20px;
        color: white;
        margin-bottom: 20px;
        span{
            color: #2eca8b;
            margin: 0 5px;
        }
        #riga{
            display: flex;
            justify-content: space-around;
            background-color: #3c4858;
            border-radius: 5px;
            padding: 1px;
            color: white;
            margin-bottom: 15px;
            .btn{
                display: flex;
                justify-content: center;
                padding: 10px;
                width: 100%;
            }
            .active{
                background-color: #202942;
                border-radius: 5px;
            }
        }
    }
}
</style>