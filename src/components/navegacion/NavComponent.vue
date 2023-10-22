<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary" style="background-color: #000 !important;">
    <div class="container-fluid">
    <a class="navbar-brand title-app" href="#" style="color:rgb(252, 248, 248) !important;">
        <i class="bi bi-cart4 logo-color" id="logo-compras"></i>
        Compras para el hogar S.A de C.V.</a
        >
        <button
        class="navhar-toggler"
        type="button"
        data-bs-toggles="collapse"
        data-bs-target="navbarSupporttedContent"
        aria-controls="navbarSupporttedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
        >
        
    </button>
    <div class="collapsee navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
                <a class="nav-link active title-app " aria-current="page" href="#" style="color: white;">
                    <i class="fas fa-laptop-house"></i>
                    Home
                </a>
            </li>
            <li class="naw-item">
                <router-link to="/from" class="nav-link title-app" style="color: white;">
                    <i class="fas fa-calendar-plus"></i>
                    Captura de Datos
                </router-link>    
            </li>
            <li class="nav-item">
                <router-link to="/from-articulos" class="nav-link title-app" style="color: white;">
                    <i class="far fa-newspaper"></i>
                    Articulos
                </router-link
            >
            </li>
            <li class="nav-item dropdown">
                <router-link class="nav-link dropdown-toggle title-nav" to="/proveedores" tag="a" role="button" data-bs-toggle="dropdown" area-expanded="false">
                    <i class="fas fa-user-ninja"></i>
                    Proveedores
                </router-link>
                <ul class="dropdown-menu">
                    <li> <router-link to="/manager-proveedores" class="nav-link title-app"><i class="far fa-thumbs-up"></i>Administracion</router-link></li>
                    <li> <a class="dropdown-item" href="#">Agregar</a></li>
                    <li> <hr class="dropdown-divider"/></li>
                    <li> <a class="dropdown-item" href="#">Manager</a></li>
                </ul>
           </li>
            <li class="nav-item">
                <a class="nav-link disabled "  aria-disabled="true" style="color: white;">
                    <i class="fas fa-bell-slash"></i>
                    Disabled
                </a> 
            </li>
        </ul>
        <form class="d-flex" role="search" style="color: white;"> 
            <i class="fas fa-search"></i>
            <input 
            id="busqueda"
            class="from-control me-2"
            type="search"
            placeholder="search"
            aria-label="Search"
            />
            <button class="btn btn-outline-success " type="submit" id="button">Search </button>
        </form>
    </div>
    </div>
</nav>
</template>
<script>

export default{
    name: "NavComponent",
};
</script>
<style scoped>
.nav-color{
    background-color: #eb29b8!important;
    color:white!important;
}
.title-nav{
    color: #ffffff !important;
    font-family:'Roboto','sans-serif';
    font-weight: 400;
}
#busqueda{
    color: white;
    padding-left: 5px; 
    background-color: transparent;
    
}
#busqueda::placeholder{
    color: white;

}
#button {
    color: #000000; 
    background-color: #ffffff;
}

#button:hover{
    background-color:#eb29b8;
    color: white;
}


</style>