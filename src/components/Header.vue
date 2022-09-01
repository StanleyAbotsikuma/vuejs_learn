<template>
    <div class="header">
        <ul>
            <li>Home Page</li>
            <li>About Page</li>
            <li> Contact</li>
        </ul>

    </div>
    <DataVue/>
    
</template>
<script>
    import DataVue from './Data.vue';
export default {
    components:{
        DataVue,
    }
}
</script>

<style>
.header
{
    width: 100%;
    height: 100%;
margin-top: 90px;}
</style>