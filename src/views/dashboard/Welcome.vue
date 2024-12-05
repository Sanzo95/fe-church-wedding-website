<script setup>
import { onBeforeMount } from 'vue';
import { disabilitaEventiDevTools, router } from '../../plugins/router';

onBeforeMount(() => {
  const route = useRoute();
  }
);

const labelWelcome = ref();
onMounted(() => {
  disabilitaEventiDevTools();
    labelWelcome.value = 'Ci farebbe molto piacere se fossi presente alla celebrazione del nostro matrimonio in chiesa e al momento del grande "SI"!';

});
</script>


<template>
  <VCard class="position-relative">
    <VCardText>
      <div class="mb-2">
        <h5 class="text-h5 v-text-wrap-justify" style="text-transform: capitalize !important;">
          Benvenutə <span class="text-high-emphasis">🎉</span>
        </h5>
        <div class="text-body-1">
          <span class="v-text-wrap-justify">{{ labelWelcome }} </span>
        </div>
      </div>
    </VCardText>
  </VCard>
</template>
