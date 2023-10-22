<template>
    <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle title-app" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            <i class="bi bi-bag-check logo-color"></i>
            Proveedores
        </a>
        <ul class="dropdown-menu">
            <router-link to="/manager-proveedores" class="bav-link title-app">Registrar</router-link>
            <li><a class="dropdown-item" href="#">Proveedores</a></li>
            <li><a class="dropdown-divider" href="#"></a></li>
            <li><a class="dropdown-item" href="#">Clientes</a></li>
        </ul>
    </li>
</template>
<script>
export default {
    name: 'ProveedorCatalogoComponent'
}
</script>