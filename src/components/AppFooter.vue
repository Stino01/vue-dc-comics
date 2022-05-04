<template>
    <footer>
        <FooterSub />
        <FooterInfo />
        <FooterSing />
    </footer>
</template>

<script>
import FooterSub from "./footercomponents/FooterSub.vue"
import FooterInfo from "./footercomponents/FooterInfo.vue"
import FooterSing from "./footercomponents/FooterSing.vue"

export default {
  name: 'AppFooter',
  components: {
    FooterSub,
    FooterInfo,
    FooterSing,
  }
}
</script>

<style lang="scss">
  @import "../style/variables.scss";
</style>