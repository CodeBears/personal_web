<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About Me</router-link> |
    <router-link to="/contact">Contact</router-link>
  </div>
  <router-view />
</template>

<style lang="sass">
body
  height: 100%
  background-color: black
  color: #20C20E

#app
  font-family: monospace, Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
#nav
  padding: 30px

#nav a
  font-weight: bold
  color: #2c3e50

#nav a.router-link-exact-active
  color: #20C20E

h2
  color: rgb(145, 45, 45)

.typerText
  font-size: 2em
  text-align: left
  color: #20C20E
p
  text-align: left
#typer
  border-right: .05em solid
  animation: caret 1s steps(1) infinite
  color: #20C20E

// #helloWorld
//   position: relative
//   left: 100px
svg
  fill: currentColor
  color: #20C20E

#typerBlock
  margin: 0 10%

.flexContainer
  display: flex
  flex-wrap: wrap
  justify-content: space-evenly
  width: 80%
  margin: 0px auto

.skillBlock
  width: 280px
  height: 200px
  margin: 5px
  font-size: 1rm
  border: 3px solid
  padding-top: 10px
  border-radius: 10px

.skillContent
  text-align: left
@keyframes caret
  50%
    border-color: transparent
</style>
