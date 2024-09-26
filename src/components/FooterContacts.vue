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
    }
},
}
</script>

<template>
    <div class="club-logo">
        <img src="../assets/logo-footer-football.png" alt="logo-club">
    </div>
    <div class="club-contacts">
        <div class="location">
            <i class="bi bi-geo-alt"></i>
            <span>{{ contacts[0].address }}</span>
        </div>
        <div class="telephone-number">
            <i class="bi bi-telephone"></i>
            <span>{{ contacts[1].telephone }}</span>
        </div>
        <div class="e-mail">
            <i class="bi bi-envelope"></i>
            <span>{{ contacts[2].email }}</span>
        </div>
        <div class="social">

        </div>
    </div>
</template>

<style scoped>
img {
    width: 60px;
}

span {
    color: white;
}

.bi {
    color: white;
}
</style>