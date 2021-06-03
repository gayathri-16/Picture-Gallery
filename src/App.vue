<template>
    <div class="container">
        <meta name="viewport" content="width=device-width, initial-scale=1">
       <div class="poster-detail">
           <img class="poster" src="./assets/photo9.jpg" alt="">
           <h1>Rodney Cotton</h1>
           <h3>Helsinki, Finland</h3>
           
           <button class="btn">100 <p>Post</p> </button>
           <button class="btn"> 2,242<p>Follower</p></button>
           <button class="btn">1,432<p>Following</p></button>
       </div>
       <div class="gallery">
           <div class="gallery-item"> <img  src="./assets/photo1.jpg" ></div>
           <div class="gallery-item"> <img  src="./assets/photo2.jpg" ></div>
           <div class="gallery-item"> <img  src="./assets/photo3.jpg" ></div>
           <div class="gallery-item"> <img  src="./assets/photo4.jpg" ></div>
           <div class="gallery-item"> <img  src="./assets/photo5.jpg" ></div>
           <div class="gallery-item"> <img  src="./assets/photo6.jpg" ></div>
          
       </div>

       <section><span></span></section>
</div>
</template>

<script>
function createBubble(){
  const section = document.querySelector('section')
  const createElement = document.createElement('span')
  var size = Math.random()*60;

  createElement.style.width = 20 + size + 'px';
   createElement.style.height = 20 + size + 'px';
    createElement.style.left = Math.random() * innerWidth + "px";
    section.appendChild(createElement);

    setTimeout(()=>{
      createElement.remove()
    },4000)

}
setInterval(createBubble,50)

    export default {
        
    }
</script>

<style>
.container{
    background: black;
}
.poster-detail{
    align-items: center;
    justify-items: center;
    margin-left:43rem;
    margin-top:-15px;
    padding:25px;
    width:600px;
    height:300px;
}
.poster{
    
    width:100px;
    height:100px;
    border-radius:10px;
    text-align: center;
}
h1{
    font-size:18px;
    margin-left:-10px;
    color:#fff;
    margin-top:-1px;
    font-family: 'Poppins',sans-serif;
}
h3{
    margin-top:-0.8rem;
    margin-left:8px;
    color:rgba(248, 244, 244, 0.534);
    font-size:12px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif; 
}
p{
    
    margin-top:0.5rem;
    color:rgba(102, 101, 101, 0.904);
    font-size:12px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}
.btn{
    width:75px;
    height:50px;
    border-radius:10px;
    background: rgb(211, 201, 201);
    margin-right:5rem;
    margin-left:-4rem;
    padding: 10px;
    border-style:none;
    font-weight: bold;
    font-size:12px;
}
img{
    max-width:100%;
    height:auto;
     border-radius:15px;
    }
.gallery{
    margin: 0 0.65rem;

}
.gallery-item{
    height:auto;
    margin:0.5rem;
}
.gallery-item img{
    width:100%;
    height:100%;
    object-fit: cover;
   
}
.gallery{
  margin-top:-6rem;
  display:grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(1,300px);
  grid-auto-flow: row dense;
  margin-left:-4rem;
 }
.gallery-item{
       margin:0rem;
}
.gallery-item:first-child{
    grid-row:  span 1;
    width:250px;
    margin-left:25rem;
    height:250px;

}
.gallery-item:nth-child(2){
    margin-left:-22rem;
    width:600px;
    height:250px;

}
.gallery-item:nth-child(3){
    width:615px;
    height:250px;
    margin-left:25rem;
    margin-top:-2.2rem;

}

.gallery-item:nth-child(4){
    margin-top:14.5rem;
    width:300px;
    margin-left:-38.8rem;
}
.gallery-item:nth-child(5){
    width:300px;
    margin-top:-12rem;
    margin-left:45rem;
}
    .gallery-item:nth-child(6){
    width:240px;
    grid-column: 2/3;
    grid-row:span 2;
    margin-top:-28.7rem;
    margin-left:0.6rem;
    

}
    


@media only screen and (max-width:600px) {
.gallery{
    margin-top:3rem;
    display:grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(1,300px);
    grid-auto-flow: row dense;
    margin-left:-20rem;
    

}
.container{
    height:100vh;
    background:black;
}
.gallery-item{
    margin:0rem;
    
}
.gallery-item:first-child{
    grid-row:  span 1;
    width:100px;
    margin-left:25rem;
    height:100px;

}
.gallery-item:nth-child(2){
    margin-left:-6rem;
    width:210px;
    height:100px;

}
.gallery-item:nth-child(3){
    width:210px;
    height:100px;
    margin-left:24.8rem;
    margin-top:-12rem;

}

.gallery-item:nth-child(4){
    margin-top:-5rem;
    width:98px;
    height:100px;
    margin-left:-13rem;
}
.gallery-item:nth-child(5){
    width:98px;
    height:100px;
    margin-top:-6.3rem;
    margin-left:31.8rem;
}
    .gallery-item:nth-child(6){
    width:107px;
    grid-column: 2/3;
    grid-row:span 2;
    margin-top:-13.2rem;
    margin-left:0.5rem;
    height:210px;
    

}
.poster-detail{
align-items: center;
justify-items: center;
margin-left:11rem;
margin-top:1rem;
padding:5px;
width:350px;
height:200px;

}
.poster{
    
    width:100px;
    height:100px;
    border-radius:10px;
    text-align: center;
}
h1{
    font-size:16px;
    margin-left:-0.5rem;
    margin-top:-1px;
  
}
h3{
    margin-top:-0.5rem;
    margin-left:0.5rem;
    font-size:12px;
}
p{
   margin-top:0.2rem;
   font-size:12px;
 }
.btn{
    width:65px;
    height:50px;
    padding: 8px;
    font-size:14px;
}
img{
    width: auto;
}
}

section span:before{
   content:'';
   position:absolute;
   width:100%;
   height:100%;
   transform: scale(0.25)translate(-70%,-70%);
   background: radial-gradient(#fff,transparent);
   border-radius:50%;
 }
  section span{
   
    position:absolute;
  
    pointer-events: none;
   
    animation: animate 4s linear infinite;
  }
  @keyframes animate
  { 0%{
      transform: translateY(-1800%);
    opacity:1;
    
  }
  99%{
    opacity:1;
  }
  100%{
    transform: translateY(-10%);
    opacity:0;
  }

  }


</style>
