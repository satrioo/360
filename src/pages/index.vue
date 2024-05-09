<template>
  <div ref="viewer" id="viewer" style="width: 100vw; height: 100vh"></div>
</template>

<script>
import { Viewer } from "@photo-sphere-viewer/core";
import '@photo-sphere-viewer/core/index.css'

export default {
  name: 'PhotoSphereViewer',
  mounted() {
    new Viewer({
      container: "viewer",
      panorama: 'https://i.ibb.co/2sWtDGQ/bb.jpg',
      caption: "Preview Photo",
      touchmoveTwoFingers: true,
      mousewheelCtrlKey: true,
      defaultZoomLvl: 0
    });
  },
};
</script>