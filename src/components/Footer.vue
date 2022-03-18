<template>
  <section id="footer">
    <aside>
      <h1>Designed and built by Stella Samaranayake</h1>
      <h2>/ 2022</h2>
    </aside>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#footer {
  width: 100%;
  height: 100px;
  background-color: #451149;
  text-align: center;
}

aside {
  padding-top: 40px;
  font-family: "Karla", sans-serif;
  display: flex;
  justify-content: center;

  h1 {
    font-size: 1rem;
    color: #86196d;
  }

  h2 {
    font-size: 1rem;
    margin-left: 5px;
    color: #7c5172;
  }
}
</style>
