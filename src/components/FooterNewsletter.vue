<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
    <div class="footer-newsletter d-flex flex-column gap-1">
        <h3>Join Our Newsletter</h3>
        <p>Subscribe to be informed about important developments in our club and football world.</p>
        <input type="text" placeholder="Your Email Address">
        <button>Subscribe <i class="bi bi-arrow-right"></i></button>
    </div>
</template>

<style scoped>
    .footer-newsletter {
        flex-basis: calc(100% / 3);
    }

    h3, p {
        color: white;
    }

    input, button {
        padding: 15px 20px;
        border-radius: 40px;
    }
</style>