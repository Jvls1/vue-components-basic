<template>
  <section>
    <base-card>
      <template #header>
        <h3>{{ fullName }}</h3>
        <base-badge :type="role" :caption="role.toUpperCase()"></base-badge>
      </template>
      <p>{{ infoText }}</p>
    </base-card>
  </section>
</template>

<script>
import BaseCard from "@/components/UI/BaseCard";

export default {
  components: {BaseCard},
  props: ['fullName', 'infoText', 'role'],
};
</script>
