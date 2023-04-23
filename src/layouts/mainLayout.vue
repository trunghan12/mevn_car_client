<template>
    <div id="demo" class="" style="background: #fef5ef!important;">
        <HeaderApp />
        <div style="margin-top: 64px"></div>
        <SlideApp />
        <div class="container-fluid">
            <div class="container-cover">
                <div class="row">
                    <SideBar />
                    <slot/>
                </div>
            </div>           
        </div>
        <FooterApp />
    </div>
</template>

<script>
import HeaderApp from '../components/main/HeaderApp.vue'
import SlideApp from '../components/main/SlideApp.vue'
import SideBar from '../components/main/SideBar.vue'
import FooterApp from '../components/main/FooterApp.vue'

export default{
    name: 'mainLayout',
    components: {
        HeaderApp,
        SlideApp,
        SideBar,
        FooterApp
    }
}
</script>

<!-- <style scoped>
#demo{
    opacity: 0.8;
    background: linear-gradient(90deg, rgba(255, 255, 255, 0.1) 0%, rgba(255, 255, 255, 0.1) 100%), url(https://media.baodansinh.vn/baodansinh/2020/11/26/photo-1606393749356-16063937493641669154530.jpg);
    background-position: center;
}
</style> -->