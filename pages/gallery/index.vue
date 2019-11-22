<template>
  <div class="container">
    <div>
      <ProductZoomer
        :base-images="images"
        :base-zoomer-options="zoomerOptions"
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: {
        thumbs: [
          {
            id: 1,
            url: 'https://placehold.it/1040x1040'
          },
          {
            id: 2,
            url: 'https://placehold.it/1040x1040'
          }
        ],
        normal_size: [
          {
            id: 1,
            url: 'https://placehold.it/1040x1040'
          },
          {
            id: 2,
            url: 'https://placehold.it/1040x1040'
          }
        ],
        large_size: [
          {
            id: 1,
            url: 'https://placehold.it/1040x1040'
          },
          {
            id: 2,
            url: 'https://placehold.it/1040x1040'
          }
        ]
      },
      zoomerOptions: {
        zoomFactor: 3,
        pane: 'pane',
        hoverDelay: 300,
        namespace: 'zoomer-bottom',
        move_by_click: false,
        scroll_items: 4,
        choosed_thumb_border_color: '#dd2c00',
        scroller_position: 'bottom',
        zoomer_pane_position: 'right'
      }
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
