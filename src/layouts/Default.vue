<template>
  <div>
    <Ribbon/>
    <slot/>
  </div>
</template>

<script>
import './index.css';
import '../components/Ribbon.vue';
import Ribbon from '../components/Ribbon.vue';

export default {
    components: {
        Ribbon,
    }
}
</script>
