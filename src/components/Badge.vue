<template class="p-4">
  <svg-icon type="mdi" :path="path"></svg-icon>
</template>

<script>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiAccessPointNetwork } from "@mdi/js";

export default {
  name: "Badge",
  components: {
    SvgIcon,
  },
  data() {
    return {
      path: mdiAccessPointNetwork,
    };
  },
};
</script>