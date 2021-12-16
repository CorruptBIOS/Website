<template>
  <div class="theme-container">
    <div class="theme-default-content">
      <img src="https://images.rbxcdn.com/9281912c23312bc0d08ab750afa588cc.png" alt="404"  width="512">

      <h1>404</h1>
      <blockquote>{{ getMsg() }}</blockquote>
      <router-link to="/">Take me home.</router-link>
    </div>
  </div>
</template>

<script>
const msgs = [
  `There's nothing here.`,
  `How did we get here?`,
  `That's a Four-Oh-Four.`,
  `Looks like we've got some broken links.`,
  `Someone divided by zero.`,
  `Oh, a blank page.`,
  `Whoops that doesn't appear to exist.`,
  `Something isn't right here.`,
  `That page does not exist.`,
  `Are we there yet?`
]

export default {
  methods: {
    getMsg () {
      return msgs[Math.floor(Math.random() * msgs.length)]
    }
  }
}
</script>
