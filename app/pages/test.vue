import testSettings from '@/content/testpage.json';

export default class TestPage extends Vue {
  pageContent = testSettings.pageContent;
}
<template>
    <section class="test-page">
      <div v-html="$md.render(pageContent)" class="page-content markdown"></div>
    </section>
  </template>
  