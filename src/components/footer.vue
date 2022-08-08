<template>
<div>
<footer>
                <img src="../../src/assets/images/LogoEMOVI-head-retina.png" alt="" width="250">
                <p class="text-footer"><small> EMOVI, 2022</small></p>
            </footer>
</div>
</template>
<script>

export default {
  name: 'footer-emovi',
  props: {
  },
}
</script>
<style scoped>
.text-footer{
color:white
}
.text-small {
  font-size: 0.9rem;
}

a {
  color: inherit;
  text-decoration: none;
  transition: all 0.3s;
}

a:hover, a:focus {
  text-decoration: none;
}

.form-control {
  background: #212529;
  border-color: #545454;
}

.form-control:focus {
  background: #212529;
}

footer {
  background: #212529;
}
</style>