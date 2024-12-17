<template>
    <div>
        <div class="container">
            <div class="card">
                <div class="content">
                
                    <p>Ainda não tem o seu vestido tão sonhado?</p>
                    <h2>Catálogo de Vestidos</h2>
                    <p>Descubra as últimas tendências dos melhores estilistas em vestidos de noiva, trajes de noivo, acessórios e decorações alianças e muito mais. </p>
                    <p>Navegue pelo catálogo mais completo, criado e atualizado para você brilhar no Grande Dia!</p>
                    <div class="link">
                    <nav>
                        <ul>
                            <a href="https://www.closetdamay.com.br"><li>Vestido Noiva</li></a>
                            <a href="https://www.closetdamay.com.br"><li>Vestido de Festa</li></a>                            
                            <a href="https://www.closetdamay.com.br"><li>Acessórios</li></a>
                        </ul>

                     </nav>
                     
                     <nav>
                        <ul>
                            <a href="https://www.drterno.com.br/"><li>Terno Noivo</li></a>
                            <a href="https://www.drterno.com.br/"><li>Roupa de Festa</li></a>    
                        </ul>
                    </nav>
                </div>
                    <a href="https://www.closetdamay.com.br"><button class="btn-c">Ver Catalogo</button></a>
                </div>
                
                <div class="conteiner-list">
            <div class="card-list">
                <div class="img-list1">

                </div>
                <a href="https://www.constancezahn.com"  target="_blank"><h4>Atelier Noiva</h4></a>
                <p>3 Fornecedores</p>
            </div>
            <div class="card-list">
                <div class="img-list2">

                </div>
                <a href="https://www.docenoivas.com.br" target="_blank"><h4>Lojas de Noivos</h4></a>
                <p>5 Fornecedores</p>
            </div>
                       
            
            
        </div>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name: 'Catalogo'
}
</script>

<style scoped>
.btn-c{
    background-color: transparent;
    color: #bd1010;
    border: 2px solid #cc0f0f;
    cursor: pointer;
    padding: 8px 14px;
    font-weight: 500;
    border-radius: 5px;
    font-size: 1.1rem;
    margin-left: 18px;
    margin: 18px;
    
}

.btn-c:hover{
    background-color: #cc0f0f;
    color: #FFFFFF;
    transition: 0.4s;
}
.container{
    width: 100%;
    height: auto;
    display: flex;
    margin-top: 30px;
    padding-bottom: 100px;
    padding-left: 20px;
    overflow-x: hidden;
    
}
.card{
    display: flex;
}

.content{
    width: 55%;
}

.link{
    display: flex;
}

.link li{
    margin: 20px 20px;
    list-style: none;
    font-weight: 400;
}
.link a{
    text-decoration: none;
    color: #000;
    font-size: 1.1rem;
}

.link a:hover{
    text-decoration: underline;
    color: #df2626;
    transition: 0.4s;
}

.content h2{
    font-weight: 400;
    text-transform: uppercase;
    font-size: 1.4rem;
    margin: 0px 20px;
    text-shadow: 1px 1px 1px #aaaaaa69;
  }
  
  .content p{
    margin: 10px 20px  ;
    padding-right: 80px;
    font-size: 1.2rem;
    color: #242421d5;
  }

.conteiner-list{
    width: 45%;
    height: auto;
    display: flex;
    justify-content: end;
    margin-top: 75px;
    border-radius: 70px 0px 0px 70px;
    margin-right: 40px;
}
.card-list p{
    color: #0f0f0faa;    
    margin-left: 50px;
}
.card-list h4{
    margin-left: 50px;
    font-weight: 400;
}
.card-list a{
    color: #000000;
    text-decoration: none;
    font-weight: 400;
}

.card-list a:hover{
    color: #df2626;
    text-decoration: underline;
    font-weight: 500;
    transition: 0.4s;
}
.conteiner-list .img-list1{
    background-image: url('public/img/Atelier.jpg');
    background-size: cover;
    background-repeat: no-repeat ;
    width: 170px;
    height: 220px;
    margin: 20px;
    overflow: hidden;
    border-radius: 10px;
    filter: grayscale(60%);
    transition: .6s;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}
.conteiner-list .img-list1:hover{
    background-size: 110% ;
    filter: none;    
    transition: .6s;
}

.conteiner-list .img-list2{
    background-image: url('public/img/terno.jpg');
    background-size: cover;
    background-repeat: no-repeat ;
    width: 170px;
    height: 220px;
    margin: 20px;
    overflow: hidden;
    border-radius: 10px;
    filter: grayscale(60%);
    transition: .6s;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}
.conteiner-list .img-list2:hover{
    background-size: 110% ;
    filter: none;    
    transition: .6s;
}




</style>