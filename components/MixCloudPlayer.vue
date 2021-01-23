<template>
  <div id="mixcloud-player">
    <!-- My player API -->
    <iframe
      width="100%"
      height="120"
      src="https://www.mixcloud.com/widget/iframe/?hide_cover=1&feed=%2Fseparationpoints%2Ffridays-at-the-loft-latin-special-20-11-2020%2F"
      frameborder="0"
      allow="autoplay"
    ></iframe>
  </div>
</template>




<style>
</style>

<script>
import MixCloudPlayer from "../components/MixCloudPlayer";

export default {
  components: {
    MixCloudPlayer,
  },

  data() {
    return {};
  },
};
</script>




