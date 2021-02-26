<template>
  <q-layout view="hHh Lpr lff">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />

        <q-toolbar-title>
          TwD3-Web
        </q-toolbar-title>

        <div>
          <a href="https://chrome.google.com/webstore/detail/twd3/pbmcgkecchhocbndaicehjpdocoflbeg">
            <img src="https://img.shields.io/chrome-web-store/v/pbmcgkecchhocbndaicehjpdocoflbeg"/>
          </a>
        </div>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-grey-1"
    >
      <q-list>
        <q-item-label
          header
          class="text-grey-8"
        >
          Essential Links
        </q-item-label>
        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer>
      <q-toolbar>
        <q-toolbar-title />
          <div>
            The MIT License,  Copyright (c) 2020-2021 Atria64. All Rights Reserved.
          </div>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
import EssentialLink from 'components/EssentialLink.vue'

const linksData = [
  {
    title: 'TwD3 GitHub Repository',
    caption: 'github.com/Atria64/TwD3',
    icon: 'fab fa-github-square',
    link: 'https://github.com/Atria64/TwD3'
  },
  {
    title: 'Latest Release(Github)',
    caption: 'github.com/Atria64/TwD3/releases',
    icon: 'new_releases',
    link: 'https://github.com/Atria64/TwD3/releases'
  },
  {
    title: 'Download',
    caption: 'Chrome Web Store',
    icon: 'get_app',
    link: 'https://chrome.google.com/webstore/detail/twd3/pbmcgkecchhocbndaicehjpdocoflbeg'
  },
  {
    title: 'Twitter',
    caption: '@AtriaSoft',
    icon: 'fab fa-twitter',
    link: 'https://twitter.com/AtriaSoft'
  },
  {
    title: 'TwD3-Web GitHub Repository',
    caption: 'github.com/Atria64/twd3-web',
    icon: 'fab fa-github-square',
    link: 'fab fa-github-square'
  }
]

export default {
  name: 'MainLayout',
  components: { EssentialLink },
  data () {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksData
    }
  }
}
</script>
