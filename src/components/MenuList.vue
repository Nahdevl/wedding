<template>
    <div class="menu">
        <router-link to="/info" class="menu-content">
            <img :src="require('@/assets/icon/home-Regular.png')" class="icon1">
            <p>Home</p>
        </router-link>
        <router-link to="about.html" class="menu-content">
            <img :src="require('@/assets/icon/Group.png')" class="icon2">
            <p>Abot us</p>
        </router-link>
        <router-link to="images.html" class="menu-content">
            <img :src="require('@/assets/icon/image-Regular.png')" class="icon3">
            <p>Images</p>
        </router-link>
        <router-link to="list.html" class="menu-content">
            <img :src="require('@/assets/icon/Vector.png')" class="icon4">
            <p>List</p>
        </router-link>
    </div>
</template>

<script>
    export default{
        name: 'MenuList',
    }
</script>

<style type="text/css">
    /* menu*/
.menu
{
    display: flex;
    width: 100%;
    height: 56px;
    position: fixed;
    z-index: 999;
    bottom: 0;
    background: var(--primary);
    justify-content: center;
    align-items: center;
    box-shadow: 9px 3px 14px rgba(0, 0, 0,0.25)
}
.menu .menu-content
{
    margin: 0 1rem;
    flex-direction: column;
    display:flex;
    justify-content: center;
    align-items: center;
}
.menu a.menu-content:hover p
{
    color: var(--head);
}
.menu .menu-content p
{
    text-align:center;
    padding-top: 2px;
    font-size: 0.8rem;
    color: var(--button);
}
.menu .menu-content img.icon1
{
    width: 25px;
    height: 25px;
}
.menu .menu-content img.icon2
{
    width: 27px;
    height: 23px;
}
.menu .menu-content img.icon3
{
    width: 27px;
    height: 23px;
}
.menu .menu-content img.icon4
{
    width: 25px;
    height: 25px;
}
</style>