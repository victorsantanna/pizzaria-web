<template>
    <div>
        <p> C. de mensagem</p>
    </div>
    <div>
        <form action="" id="pizza-form">
            <div class="input-container">
                <label for="nome">Nome do Cliente</label>
                <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite o seu nome">
            </div>
            <div class="input-container">
                <label for="Pizza">Escolha a Massa:</label>
                <select name="pizza" id="pizza" v-model="pizza">
                <option value="">Selecione o tipo da massa</option>
                <option value="integral">Integral</option>
                </select>
            </div>
            <div class="input-container">
                <label for="recheio">Escolha o recheio:</label>
                <select name="recheio" id="recheio" v-model="recheio">
                <option value="">Selecione o tipo do recheio</option>
                <option value="integral">4 Queijos</option>
                </select>
            </div>
            <div id="opcionais-container" class="input-container">
                <label for="opcionais" id="opcionais-title">Escolha os opcionais:</label>
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
                    <span>Salame</span>
                </div>
            </div>
            <div class="input-container">
                <input type="submit" class="submit-btn" value="Criar minha Pizza">
            </div>
        </form>
    </div>
</template>

<script>
export default {
    name:"PizzaForm"
    
}
</script>

<style scoped>

#pizza-form{
    max-width: 400px;
    margin: 0 auto;
    
}

.input-container{
    display: flex;
    flex-direction: column;
    margin-bottom:20px;
   
}

label{
    font-weight: bold;
    font-family: Tahoma, sans-serif;
    margin-bottom: 15px;
    color: #333;
    padding: 5px 10px;
    border-left: 4px solid #FCBA03;
}

input, select{
    padding: 5px 10px;
    width: 400px;
}
#opcionais-container{
    flex-direction: row;
    flex-wrap: wrap;
}

#opcionais-title{
    width: 100%;
    
}

.checkbox-container{
    display: flex;
    align-items: flex-start;
    width: 50%;
    margin-bottom: 20px;

}

.checkbox-container span, 
.checkbox-container input{
    width: auto;
}

.checkbox-container span{
    margin-left: 6px;
    font-weight: bold;

}

.submit-btn{
    background-color: #222;
    color: #FCBA03;
    font-weight: bold;
    border: 2px solid #222;
    padding: 10px;
    font-size: 16px;
    font-family: Tahoma, sans-serif;
    margin: 0 auto;
    cursor: pointer;
    transition: .2s;

}

.submit-btn:hover{
    background-color: transparent;
    color: #444;
}

</style>