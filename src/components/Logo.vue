<template>
    <div class="logo">
        <h2>N & N</h2>
    </div>
</template>

<script>
    export default{
        name:'Logo',
    }
</script>

<style type="text/css">
.logo
{
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background-color: var(--primary);
    text-align: center;
    font-family: 'Dancing Script';
    font-size: 1rem;
    padding: 0.4rem;
    color: var(--button);
    z-index: 999;
}

</style>