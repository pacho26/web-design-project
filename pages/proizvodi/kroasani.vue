<template>
  <div>
    <div class="content">
      <CategoryProducts categoryName="Kroasani" :products="getCroissants" />
    </div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex';

export default {
  computed: {
    ...mapGetters(['getCroissants']),
  },
};
</script>

<style lang="scss" scoped>
.content {
  @media only screen and (max-width: 1548px) {
    margin: 0 3.3vw;
  }

  @media only screen and (max-width: 768px) {
    margin-top: 75px + 44px;
  }

  @media only screen and (max-width: 592px) {
    margin-top: 75px + 28px;
  }
}
</style>
