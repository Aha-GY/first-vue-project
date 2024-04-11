<template> 
    <div class="page">
      <div class="innerchild">
        <div class="flex-part1">
            <section class="logo">
                <img src="@/assets/logo.png" alt="social media logo">
            </section>
            <section class="madia">
                <h1> social media assistant </h1>
                <p> yengat brihan non profit organization . addis ababa ethiopia </p>
            </section>
        </div>
        <div class="part2">
                <p>
                    As a Social Media Assistant, you will work closely with the social media manager or marketing 
                    team to execute social media strategies and campaigns. You will be responsible 
                    for assisting in the creation and scheduling of engaging content, monitoring social media channels, and
                    interacting with followers.
                </p>
        </div>
        <div class="part3">
            <button id="start" @click="showButtonText('In person')"> In Person</button>
            <button id="mid"   @click="showButtonText('Education')"> Education</button>
            <button id="end"   @click="showButtonText('IT')"> IT</button>

        </div>
      </div>
    </div>
    
</template>



<style>
.page{
    background-color: gray;
    padding : 10px;
}
.madia{
    text-transform: capitalize;
    }

.innerchild{
    border-radius: 16px ;
    padding : 20px 30px;
    background-color: white;
}
.flex-part1{
        display: flex;
        /* justify-content: center ; */
        align-items: center;
    }
.logo{
    width : 60px;
    height : 60px;
    margin-right : 10px;
}
  
   
        img{
        width: 100%;
        height: 100%;
        margin-right: 30px;
    }
    button{
      padding : 10px 20px;
      margin-right: 10px;
      border-radius: 999px;
      /* border-radius: 50%; */
       

    }
    .part3 #start{
        color:green;
        border : green 1.5px solid;
    }
    .part3 #mid{
        color: rgb(218, 218, 45);
        border : rgb(216, 216, 35) 1.5px solid ;
    }
    .part3 #end{
        color: darkblue;
        border : darkblue 1.5px solid ;
    }
</style>



<script>
  export default {
    data(){
        return {

        }
    },
    methods : {
        showButtonText(text){
          console.log('the text is ',text);
        }
    }
  }
</script>