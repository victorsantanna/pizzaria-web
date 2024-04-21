<template>
   <div id="main-banner">
    <h1> Make Your Pizza</h1>
   </div>
</template>

<script>
export default {
    name:"Banner"
    
}
</script>

<style scoped>
#main-banner{
    background-image: url('/public/img/pizza.jpg');
    background-position: 0 -250px;
    background-size: cover;
    height: 350px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
}

#main-banner h1{
    color:#FCBA03;
    text-align: center;
    font-size: 60px;
    font-family: Tahoma, sans-serif;
    background-color: #222;
    padding: 20px 40px;
    opacity: 0.8;   
    border-radius: 0 30px 30px 0; 

}


</style>