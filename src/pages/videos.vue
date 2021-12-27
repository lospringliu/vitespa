<script setup lang="ts">
import { ref, onMounted } from 'vue'

const video = ref(null)
const videoid = ref('3P1CnWI62Ik')
onMounted(() => {
  // window.console.log(video.value)
  // const testHash = 'mbGtJg23skhvFmu9mJiePVByhfzu5rwo74MEkVDYAmF5T'
  const testHash = 'QmdpAidwAsBGptFB3b6A9Pyi5coEbgjHrL3K2Qrsutmj9K'
  // const testHash = 'QmbrwEH4AEQhUN929yPy4j5B2PfQYk3JJyG8iq7HVoXbia'
  window.Hls.DefaultConfig.loader = window.HlsjsIpfsLoader
  window.Hls.DefaultConfig.debug = false
  if (window.Hls.isSupported()) {
    // const video = document.getElementById('video')
    const hls = new window.Hls()
    hls.config.ipfs = window.node
    hls.config.ipfsHash = testHash
    hls.loadSource('master.m3u8')
    hls.attachMedia(video.value)
    hls.on(window.Hls.Events.MANIFEST_PARSED, () => {})
  }
})
</script>

<template>
  <div class="flex items-center justify-center">
    <Youtube
      :src="videoid"
    />
  </div>
  <div class="flex items-center justify-center">
    <vue-plyr class="w-full aspect-video">
      <div class="aspect-video" data-plyr-provider="youtube" data-plyr-embed-id="bTqVqk7FSmY"></div>
    </vue-plyr>
  </div>
  <div class="flex items-center justify-center">
    <video ref="video" class="w-full aspect-video" controls></video>
  </div>
  <div class="flex items-center justify-center">
    <vue-plyr class="w-full aspect-video">
				<iframe
					src="https://www.youtube.com/embed/bTqVqk7FSmY?amp;iv_load_policy=3&amp;modestbranding=1&amp;playsinline=1&amp;showinfo=0&amp;rel=0&amp;enablejsapi=1"
					allowfullscreen
					allowtransparency
					allow="autoplay"
				></iframe>
		</vue-plyr>
  </div>
</template>
