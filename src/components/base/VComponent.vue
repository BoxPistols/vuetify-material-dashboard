<template>
  <section class="mb-12 text-center">
    <h1
      class="font-weight-normal mb-2 headline"
      v-text="`Vuetify ${heading}`"
    />

    <span
      class="font-weight-normal subtitle-1"
    >
      Please checkout the
      <a
        :href="`https://vuetifyjs.com/${link}`"
        rel="noopener"
        target="_blank"
        class="secondary--text"
        style="text-decoration:none;"
      >
        full documentation
      </a>
    </span>
  </section>
</template>

<script>
  export default {
    name: 'VComponent',

    props: {
      heading: {
        type: String,
        default: '',
      },
      link: {
        type: String,
        default: '',
      },
    },
  }
</script>
