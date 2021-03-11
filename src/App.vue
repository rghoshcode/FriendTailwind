<template>
    <div>
        <HeaderComponent></HeaderComponent>
        <section class="h-screen max-w-screen-xl my-0 mx-auto" >
            <header class="flex justify-center p-10">
                <h1 class="text-xl" >My Friends</h1>
            </header>
            <ul class="flex justify-start">
                <friend-contact id="manuel" name="lorenz manuel" phone="09867823" email="manu@web.de"></friend-contact>
                <friend-contact id="peyman" name="peyman g" phone="2952385239525" email="peym@web.de"></friend-contact>
            </ul>
        </section>
        <FooterComponent></FooterComponent>
    </div>
</template>

<script>
    import FriendContact from './components/FriendContact';
    import HeaderComponent from './components/HeaderComponent';
    import FooterComponent from './components/FooterComponent';

    export default {
        components : { FriendContact, HeaderComponent, FooterComponent },
        data(){
            return {
                id : '',
                name : '',
                phone : '',
                email : '',
                isFavorit: false,
            };
        },
    };
</script>

