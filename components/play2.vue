<template>
  <div id="mixcloud-player">
    <!-- My player API -->
    <iframe
      width="100%"
      height="120"
      src="https://www.mixcloud.com/widget/iframe/?hide_cover=1&amp;classic=1&amp;dark=1&amp;autoplay=0&amp;feed=https%3A%2F%2Fwww.mixcloud.com%2Fseparationpoints%2F038-spaven-x-sandunes-ep-brazilian-funk-and-some-more-bossa-nova-classic-brazilian-vibes%2F"
      frameborder="0"
      allow="autoplay"
    ></iframe>
  </div>
</template>

<script>
var promise = Mixcloud.FooterWidget(
  "/separationpoints/038-spaven-x-sandunes-ep-brazilian-funk-and-some-more-bossa-nova-classic-brazilian-vibes/"
);
promise.then(function (widget) {
  // Put code that interacts with the widget here e.g.
  widget.events.pause.on(pauseListener);
});

export default {
  data() {
    return {};
  },
};
</script>




  head() {
      return {
           script: [
          {
            rel: 'javascript',
            src:
              '//widget.mixcloud.com/media/js/widgetApi.js'
          },

          {
            rel: 'javascript',
            src:
            // Mixcloud footer widget //
            '//widget.mixcloud.com/media/js/footerWidgetApi.js'
     
          },

        ],

      }

 
   }

};

// Mixcloud footer widget Mixcloud.FooterWidget is the object which you can pass parameters to //

</script>

<style scoped>
</style>

