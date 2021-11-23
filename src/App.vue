<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/ability">My Ability</router-link> |
    <router-link to="/about">About Me</router-link> |
    <a  href="https://www.linkedin.com/in/johnny-chen-6a4094188/" style="vertical-align:middle" target="_blank"><svg class="navSvg" enable-background="new 0 0 56.693 56.693" height="25" viewBox="0 0 56.693 56.693" width="25" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><g><path d="M30.071,27.101v-0.077c-0.016,0.026-0.033,0.052-0.05,0.077H30.071z"/><path d="M49.265,4.667H7.145c-2.016,0-3.651,1.596-3.651,3.563v42.613c0,1.966,1.635,3.562,3.651,3.562h42.12   c2.019,0,3.654-1.597,3.654-3.562V8.23C52.919,6.262,51.283,4.667,49.265,4.667z M18.475,46.304h-7.465V23.845h7.465V46.304z    M14.743,20.777h-0.05c-2.504,0-4.124-1.725-4.124-3.88c0-2.203,1.67-3.88,4.223-3.88c2.554,0,4.125,1.677,4.175,3.88   C18.967,19.052,17.345,20.777,14.743,20.777z M45.394,46.304h-7.465V34.286c0-3.018-1.08-5.078-3.781-5.078   c-2.062,0-3.29,1.389-3.831,2.731c-0.197,0.479-0.245,1.149-0.245,1.821v12.543h-7.465c0,0,0.098-20.354,0-22.459h7.465v3.179   c0.992-1.53,2.766-3.709,6.729-3.709c4.911,0,8.594,3.211,8.594,10.11V46.304z"/></g></svg></a> |
    <a  href="https://github.com/CodeBears" style="vertical-align:middle" target="_blank"><svg class="navSvg"  enable-background="new 0 0 24 24" height="25" viewBox="0 0 24 24" width="25" xmlns="http://www.w3.org/2000/svg"><path d="m12 .5c-6.63 0-12 5.28-12 11.792 0 5.211 3.438 9.63 8.205 11.188.6.111.82-.254.82-.567 0-.28-.01-1.022-.015-2.005-3.338.711-4.042-1.582-4.042-1.582-.546-1.361-1.335-1.725-1.335-1.725-1.087-.731.084-.716.084-.716 1.205.082 1.838 1.215 1.838 1.215 1.07 1.803 2.809 1.282 3.495.981.108-.763.417-1.282.76-1.577-2.665-.295-5.466-1.309-5.466-5.827 0-1.287.465-2.339 1.235-3.164-.135-.298-.54-1.497.105-3.121 0 0 1.005-.316 3.3 1.209.96-.262 1.98-.392 3-.398 1.02.006 2.04.136 3 .398 2.28-1.525 3.285-1.209 3.285-1.209.645 1.624.24 2.823.12 3.121.765.825 1.23 1.877 1.23 3.164 0 4.53-2.805 5.527-5.475 5.817.42.354.81 1.077.81 2.182 0 1.578-.015 2.846-.015 3.229 0 .309.21.678.825.56 4.801-1.548 8.236-5.97 8.236-11.173 0-6.512-5.373-11.792-12-11.792z"/></svg></a>
  </div>
  <router-view />
</template>
<style lang="sass">
$type-green: #20C20E
$not-active-color: #2C3E50
body
  height: 100%
  background-color: black
  color: $type-green

#app
  font-family: monospace, Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
#nav
  padding: 30px

#nav a
  font-weight: bold
  color: $not-active-color
  &:hover
    color: darken($type-green, 10%)

#nav a.router-link-exact-active
  color: $type-green

.navSvg:hover
  color: darken($type-green, 10%)
h2
  color: rgb(145, 45, 45)

.typerText
  font-size: 2em
  text-align: left
  color: $type-green
p
  text-align: left
#typer
  border-right: .5em solid
  animation: caret 1s steps(1) infinite
  color: $type-green

svg
  fill: currentColor
  color: $type-green

.commonContainer
  width: 80%
  max-width: 900px
  margin: 0px auto

.flexContainer
  display: flex
  flex-wrap: wrap
  justify-content: space-evenly
  width: 100%
  overflow: hidden
  position: relative

.skillBlock
  width: 280px
  height: 200px
  margin: 5px
  font-size: 1rm
  border: 3px solid
  padding-top: 10px
  border-radius: 10px
.blackBlock
  position: absolute
  background: black
  width: 1000px
  height: 80vh
  top: 0px
  animation: fadein 1.5s
  animation-timing-function: ease-in-ease-in-out

.skillContent
  text-align: left
@keyframes caret
  50%
    border-color: transparent

@keyframes fadein
    from
      top: 0px
      opacity: 1
    to
      top: 1000px
      opacity: 0

</style>
