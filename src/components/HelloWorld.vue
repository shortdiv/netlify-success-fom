<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <form
      name="contact-form"
      class="contact-form"
      method="POST"
      data-netlify="true"
      action="/custom"
    >
      <input type="hidden" name="form-name" value="contact-form" />
      <label> name: </label>
      <input type="text" name="name" class="input" />
      <label> email: </label>
      <input type="email" name="email" class="input" required />
      <label> message: </label>
      <textarea name="message" class="textarea" placeholder="message">
      </textarea>
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
