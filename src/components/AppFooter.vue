<script>
import FooterContacts from './FooterContacts.vue';
import FooterLinks from './FooterLinks.vue';
import FooterNewsletter from './FooterNewsletter.vue';
import FooterRights from './FooterRights.vue';

export default {
    name: 'AppFooter',
components: {
    FooterContacts,
    FooterNewsletter,
    FooterLinks,
    FooterRights
},
data() {
    return {
        contacts: [
            {
                address: 'New Jersey, USA' 
            },
            {
                telephone: '+1 (234) 567 89 10'
            },
            {
                email: 'example@example.com'
            }
        ]
    }
},
methods: {

}
}
</script>

<template>
    <footer>
        <div class="general-components">
            <div class="footer-top">
                <FooterContacts
                    :contacts="contacts"
                />
                <FooterNewsletter/>
                <FooterLinks/>
            </div>
            <div class="footer-bottom">
                <FooterRights/>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
footer {
    height: 400px;
    background-image: url(../assets/footer-bg-football.jpg);
}

.footer-top {
    display: flex;
    justify-content: space-between;
    gap: 40px;
}
</style>
