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
    <div class="footer-contacts">
        <div class="club-logo">
            <img src="../assets/logo-footer-football.png" alt="logo-club">
        </div>
        <div class="club-contacts">
            <div class="location d-flex gap-3">
                <i class="bi bi-geo-alt"></i>
                <span>{{ contacts[0].address }}</span>
            </div>
            <div class="telephone-number d-flex gap-3">
                <i class="bi bi-telephone"></i>
                <span>{{ contacts[1].telephone }}</span>
            </div>
            <div class="e-mail d-flex gap-3">
                <i class="bi bi-envelope"></i>
                <span>{{ contacts[2].email }}</span>
            </div>
            <div class="social d-flex gap-3">
                <i class="bi bi-facebook"></i>
                <i class="bi bi-instagram"></i>
                <i class="bi bi-twitter"></i>
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