<template>
  <img
    width="100%"
    :src="val.url">
</template>

<script>
import braidBgStyle from './style.vue'
const WIDGET_NAME = 'braid-bg'

export default {
  name: WIDGET_NAME,
  icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smartphone"><rect x="5" y="2" width="14" height="20" rx="2" ry="2"></rect><line x1="12" y1="18" x2="12" y2="18"></line></svg>',
  title: '背景图',
  panel: braidBgStyle,
  setting: {
    type: WIDGET_NAME,
    isUpload: true,
    href: '',
    belong: 'page'
  },
  props: [
    'val'       // 图片对象
  ]
}
</script>
