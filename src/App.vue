<template>
  <div id="app">
    <div class="container">
      <header>
        <div id="nav">
          <div id="logo">
            PlowPumpService
          </div>
          <div class="spacer"></div>
          <div id="links">
            <router-link to="/">Home</router-link>
            <router-link to="/about">About</router-link>
            <router-link to="/shop">Shop</router-link>
          </div>
        </div>
      </header>
      <router-view/>
      <footer>
        © PlowPumpService 2020
      </footer>
    </div>
  </div>
</template>

<style lang="sass">
body
  margin: 0

#app
  font-family: Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50

.container
  width: 1000px
  margin: 0 auto

#nav
  display: flex
  flex-direction: row
  padding: 20px 10px
  align-items: center

  #logo
    color: blue
    font-weight: bold
    font-size: 24px

  .spacer
    flex-grow: 1

  a
    font-weight: bold
    color: #2c3e50
    margin: 0 10px
</style>
