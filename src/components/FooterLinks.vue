<script>
export default {
  data() {
    return {
      
    }
  },
  props: {
    educationLinks: {
        type: Array,
        required: true
    },
    quickLinks: {
        type: Array,
        required: true
    }
    },
}
</script>

<template>
    <div class="footer-links">
        <div class="container container-flex">
            <div class="education-section">
                <h4>Education</h4>
                <section class="education-links" v-for="(educationLink, index) in educationLinks" :key="index">
                    <a href="#">{{ educationLink }}</a>
                </section>
            </div>
            <div class="quick-section">
                <h4>Quick Links</h4>
                <section class="quick-links" v-for="(quickLink, index) in quickLinks" :key="index">
                    <a href="#">{{ quickLink }}</a>
                </section>
            </div>
        </div>
    </div>
</template>

<style scoped>
.footer-links {
    flex-basis: calc(100% / 3);
}

.container-flex {
    display: flex;
    gap: 30px;
    justify-content: end;
}

h4 {
    color: white;
}

a {
    text-decoration: none;
    text-transform: uppercase;
    color: white;
}
</style>