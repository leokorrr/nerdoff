<template>
    <div class="menu">
        <div class="menu__header">
            <h1 class="menu__title"><span class="color-purple">Nerd</span>Off</h1>
        </div>
        <div class="menu__actions">
            <div class="menu__action"><button class="project-btn">Create post</button></div>
            <div class="menu__action"><button class="menu__icon-btn"><img src="../../img/icons/notification.svg" alt=""></button></div>
            <div class="menu__action"><button class="menu__icon-btn"><img src="../../img/icons/menu-icon.svg" alt=""></button></div>
        </div>
        <Sidemenu />
    </div>
</template>

<script>
import Sidemenu from './Sidemenu.vue';

export default {
    name: 'Menu',
    components: {
        Sidemenu 
    }    
}
</script>