<template>
  <div class="welcome">
    <h1>the wedding</h1>
    <h2>Nahrul <img src="img/cincin1.png" alt=""> Nissa</h2>
    <router-link to="/info" >Buka Undangan</router-link>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import bunga2 from '@/assets/img/2bunga.png'

export default {
  name: 'HomeView'
}
</script>

<style type="text/css">
  :root{
    --button: #B95C50;
    --head: #965a00;
    --primary: #fedfe3;
    --secondary: #deb3ad;
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
}

.welcome
{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100vw;
    height: 100vh;
    background: var(--primary);
}

.welcome h1
{
    position: absolute;
    font-family: 'Caladea';
    font-size: 1.3rem;
    text-transform: uppercase;
    font-weight: 400;
    line-height: 28px;
    top: 5.5rem;
    color: var(--button);
}
.welcome h2::after
{
    content: '';
    /* margin-top: 25px; */
    position: absolute;
    width: 226px;
    height: 303px;
    left: 0px;
    top: -120px;
    background: url('@/assets/img/2bunga.png');
    background-repeat: no-repeat;
    background-size: 15rem;
}
.welcome h2
{
    position: relative;
    font-family: 'Dancing Script';
    font-weight: 400;
    /* margin-top: 50px; */
    font-size: 2rem;
    line-height: 110%;
    text-transform: uppercase;
    color: var(--head);
}
.welcome a
{
    background-color: var(--button);
    display: inline-block;
    padding: 0.6rem 4rem;
    border-radius: 1rem;
    position: relative;
    top: 11rem;
    text-transform: uppercase;
    color: #fff;
    transition: 0.5s;
}
.welcome a:hover
{
    background-color: var(--secondary);
    color: var(--button);
}
</style>
