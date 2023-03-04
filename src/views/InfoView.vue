<template>
	<logo></logo>
	<section id="info">
	    <div class="hero">
	        <!-- <img src="../img/hero2.png" alt=""> -->
	        <h2>the wedding</h2>
	        <h1>nahrul & nissa</h1>
	    </div>
	    <div class="akad">
	        <img :src="require('@/assets/img/wedding-rings 1.png')" alt="" class="icon">
	        <h1>Akad nikah</h1>
	        <p><i data-feather="calendar"></i>Monday, February 9th 2023</p>
	        <p><i data-feather="clock"></i>07.00 PM</p>
	        <p><i data-feather="map-pin"></i>Dimana Aja yang Penting SAH</p>
	        <a href="#">Open Map</a>
	    </div>
	    <div class="akad">
	        <img :src="require('@/assets/img/cheers 1.png')" alt="" class="icon">
	        <h1>Resepsi</h1>
	        <p><i data-feather="calendar"></i>Monday, February 9th 2023</p>
	        <p><i data-feather="clock"></i>07.00 PM</p>
	        <p><i data-feather="map-pin"></i>Dimana Aja yang Penting SAH</p>
	        <a href="#">Open Map</a>
	    </div>
    </section>

    <menuList></menuList>
</template>



<script>
import logo from '@/components/Logo.vue'
import menuList from '@/components/MenuList.vue'

export default {
  name: 'InfoView',
  components: {
  	logo,
  	menuList,
  }
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

section#info
{
    background: var(--secondary);
    height: 1000px;
    display: flex;
    flex-direction: column;
    /* justify-content: center; */
    align-items: center;
}

.hero
{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: url('@/assets/img/hero2.png');
    /* position: relative; */
    background-size: contain;
    background-repeat: no-repeat;
    width: 100%;
    height: 253px;
    background-position: center;
    margin-top: -1rem;
}

.hero h2
{
    font-size: 0.8rem;
    text-transform: uppercase;
    font-weight: 400;
    font-family: 'Caladea';
    color: #fff;
    line-height: 28px;
    font-feature-settings: 'ordn' on;
}
.hero h1
{
    font-size: 1rem;
    text-transform: uppercase;
    color: #fff;
    font-family: 'Caladea';
    font-weight: 400;
    line-height: 28px;
    letter-spacing: 0.30em;
}
.akad::before
{
    content: '';
    background: url('@/assets/img/bunga.png');
    position: absolute;
    background-repeat: no-repeat;
    top: -30px;
    left: 15px;
    width: 100%;
    height: 100%;
}
.akad::after
{
    content: '';
    position: absolute;
    left: 16px;
    width: 13rem;
    height: 18rem;
    border: 1px solid #965a00;
}
.akad
{
    position: relative;
    width: 15rem;
    height: 20rem;
    background: var(--primary);
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: 1rem 0;
    box-shadow: 2px 4px 4px rgba(0, 0, 0, 0.25);
    /* align-items: center; */
}
.akad img.icon
{
    width: 53px;
    height: 53px;
    margin: 0.3rem auto;
}
.akad h1
{
    font-weight: 400;
    font-size: 2rem;
    font-family: 'Dancing script';
    margin: 0.8rem;
    color: var(--head);
    text-align: center;
    line-height: 96.5%;
}

.akad p
{
    font-weight: 400;
    font-size: 0.7rem;
    line-height: 16px;
    margin: 0 1.5rem;
    
}
.akad a
{
    background-color: var(--button);
    width: 135px;
    height: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 1rem;
    position: absolute;
    bottom: 1.7rem;
    left: 50px;
    text-transform: uppercase;
    color: #fff;
    font-size: 0.6rem;
    transition: 0.5s;
    z-index: 2;
}


</style>