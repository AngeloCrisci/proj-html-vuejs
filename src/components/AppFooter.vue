<script>
import FooterContacts from './FooterContacts.vue';
import FooterLinks from './FooterLinks.vue';
import FooterNewsletter from './FooterNewsletter.vue';
import FooterRights from './FooterRights.vue';

export default {
    name: 'AppFooter',
    props: {

},
components: {
    FooterContacts,
    FooterNewsletter,
    FooterLinks,
    FooterRights
},
data() {
    return {

    }
},
methods: {

}
}
</script>

<template>
    <footer>
        <div class="footer-top">
            <FooterContacts/>
            <FooterNewsletter/>
            <FooterLinks/>
        </div>
        <div class="footer-bottom">
            <FooterRights/>
        </div>
    </footer>
</template>

<style lang="scss">
footer {
    height: 400px;
    background-image: url(../assets/footer-bg-football.jpg);
}
</style>
