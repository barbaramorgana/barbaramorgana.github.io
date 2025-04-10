<template>
  <div class="button-links">
    <a
      v-for="platform in platforms"
      :key="platform.name"
      :href="platform.url"
      class="music-button"
      :style="{ backgroundColor: platform.color }"
      target="_blank"
      rel="noopener noreferrer"
    >
      <img :src="platform.icon" :alt="platform.name" />
      {{ platform.name }}
    </a>
  </div>
</template>

<script setup lang="ts">
const iconUri = (icon: string) => `${window.location.origin}${icon}`
const platforms = [
  {
    name: 'Spotify',
    url: 'https://open.spotify.com/',
    color: '#1DB954',
    icon: 'icons/spotify.svg',
  },
  {
    name: 'YouTube',
    url: 'https://youtube.com/',
    color: '#FF0000',
    icon: 'icons/youtube.svg',
  },
  {
    name: 'YouTube Music',
    url: 'https://music.youtube.com/',
    color: '#FF0000',
    icon: 'icons/youtube-music.svg',
  },
  {
    name: 'Amazon Music',
    url: 'https://music.amazon.com/',
    color: '#232F3E',
    icon: 'icons/amazon-music.svg',
  },
  {
    name: 'Apple Music',
    url: 'https://music.apple.com/',
    color: '#FA233B',
    icon: 'icons/apple-music.svg',
  },
]
</script>

<style scoped>
.button-links {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  justify-content: center;
  align-items: center;
  width: 100%;
  max-width: 600px;
  margin: 2rem auto;
  padding: 0 1rem;
}

.music-button {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  padding: 1rem;
  border-radius: 12px;
  color: white;
  font-weight: bold;
  text-decoration: none;
  transition: transform 0.2s ease;
  width: 100%;
  box-sizing: border-box;
  font-size: 1.1rem;
  justify-content: center;
}

.music-button img {
  width: 24px;
  height: 24px;
}

.music-button:hover {
  transform: scale(1.02);
}
</style>
