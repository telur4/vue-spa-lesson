<template>
    <div>
        <Header></Header>
        <Nav></Nav>
        <Breadcrumb></Breadcrumb>
        <ContactMain></ContactMain>
        <Footer></Footer>
    </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Header from '@/components/Header.vue';
import Nav from '@/components/Nav.vue';
import Breadcrumb from '@/components/Breadcrumb.vue';
import ContactMain from '@/components/ContactMain.vue';
import Footer from '@/components/Footer.vue';

@Component({
    components: {
        Header,
        Nav,
        Breadcrumb,
        ContactMain,
        Footer
    }
})
export default class Contact extends Vue {}
</script>