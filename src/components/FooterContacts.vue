<script>
export default {
  data() {
    return {
      
    }
  },
  props: {
    contacts: {
        type: Array,
        required: true
    },
    socials: {
        type: Array,
        required: true
    }
},
}
</script>

<template>
    <div class="footer-contacts">
        <div class="club-logo">
            <img src="../assets/logo-footer-football.png" alt="logo-club">
        </div>
        <div class="club-contacts" >
            <div :class="contact.typeOfContact" class="d-flex gap-3" v-for="(contact, index) in contacts" :key="index">
                <i :class="contact.img"></i>
                <span>{{ contact.reference }}</span>
            </div>
            <div class="social d-flex gap-3">
                <i :class="social" v-for="(social, index) in socials" :key="index"></i>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer-contacts {
    flex-basis: calc(100% / 3);
}

img {
    width: 60px;
}

span {
    color: white;
}

.bi {
    color: white;
}

.social > .bi {
    border: 1px solid white;
    padding: 2px 15px;
}
</style>