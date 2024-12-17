<template>
    <div class="main-menu">
        <div class="logo">
            <RouterLink to="/">
                <li><i class="fa-solid fa-heart" style="color: #df2626;"></i> Ai Casei!</li>
            </RouterLink>
        </div>
        <div class="menu">
            <nav id="nav" style="display: flex;">
                <ul class="nav-links">
                    <RouterLink to="/"><li>Meu casamento</li></RouterLink>
                    <RouterLink to="Espacos"><li>Espaços</li></RouterLink>
                    <RouterLink to="Noivos"><li>Noivos</li></RouterLink>
                    <RouterLink to="Servicos"><li>Serviços</li></RouterLink>
                    <RouterLink to="LuaDeMel"><li>Lua de mel</li></RouterLink>
                </ul>    
                <div class="auth-buttons" style="display: flex; margin-left: 0%">
                    <template v-if="isAuthenticated">
                        <RouterLink to="/profile" class="btn btn-login"><li>Meu Perfil</li></RouterLink>
                        <button @click="handleLogout" class="btn btn-logout"><li>Sair</li></button>
                    </template>
                    <template v-else>
                        <RouterLink to="/login" class="btn btn-login"><li>Entrar</li></RouterLink>
                        <RouterLink to="/register" class="btn btn-register"><li>Cadastrar</li></RouterLink>
                    </template>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
import { mapGetters, mapActions } from "vuex";

export default {
    name: "NavBar",
    computed: {
        ...mapGetters(["isAuthenticated"]), // Verifica se o usuário está autenticado
    },
    methods: {
        ...mapActions(["logout"]), // Mapeia a ação logout do Vuex
        handleLogout() {
            this.logout(); // Limpa o estado do usuário no Vuex
            this.$router.push("/"); // Redireciona para a página inicial
        },
    },
};
</script>




<style scoped>

.btn-logout{
    margin-left: 20px;    
    background-color: #cc0f0f;
    color: #ffffff;
    cursor: pointer;
    padding: 8px 14px;
    font-weight: bold;
    border-radius: 5px;
    font-size: 1.1rem;
    margin-left: 18px;
    border: none;
}

.auth-buttons {    
    padding-left: 340px;
}

.auth-buttons a{
    background-color: transparent;
    color: #ffffff;
    background-color: #cc0f0f;
    cursor: pointer;
    padding: 8px 14px;
    font-weight: bold;
    border-radius: 5px;
    font-size: 1.1rem;
    margin-left: 18px;
    text-decoration: none;

}

.auth-buttons a:hover{
    background-color: #911b1b;
    transition: 0.4s;

}

.btn-logout:hover{
    background-color: #911b1b;
    transition: 0.4s;

}

.auth-buttons li{
    list-style: none;
    
    font-weight: 500;
}

.logo{
    margin-top: 5px;
}

</style>

