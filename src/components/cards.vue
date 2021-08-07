<template>
   <div class="cards">
       <a :href="anime.url" target="_blank">
           <img :src="anime.image_url" alt=""  />
       <h3>{{anime.title}}</h3>
       </a>
       

   </div>
</template>
<script>
export default {
    props: ['anime']
}
</script>

<style lang="scss" scoped>


.cards{
    flex: 100%;
    width: 50%;
    max-width: 33%;
    padding: 0px 8px;
    border-radius: 16px;

    img{
    height: 300px;
    width: 250px;
    object-fit: cover;
    border-radius: 16px;
    box-shadow: 0px 10px 14px rgba(0, 0, 0, 0.15);
    transition: 0.4s;
    }

     h3{
        padding: 16px;
        color: #313131;
        transition: .4s;
    }
    &:hover{

        img{
            
            transform: scale(1.05);
        }
        h3{
            color: #24C444;
        }
    }

    
}

   
    
     


</style>