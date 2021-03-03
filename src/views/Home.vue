<template>
    <div class="Home">
    <div id='typerBlock'>
      <p class="typerText" id="myName"></p>
      <p class="typerText" id="helloWorld"></p>
      <p>oh yeah</p>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Home',
  mounted() {
    const myName = 'JOHNNY CHEN';
    const helloWorld = 'Hello World!!!';

    function typeHello(i) {
      if (i === helloWorld.length) {
        return;
      }
      document.getElementById('helloWorld').innerHTML = `${helloWorld.substring(0, i + 1)}<span id="typer" aria-hidden="true"></span>`;
      setTimeout(() => {
        typeHello(i + 1);
      }, 200);
    }
    function typeName(i) {
      if (i === myName.length) {
        document.getElementById('myName').innerHTML = `${myName.substring(0, i + 1)}`;
        typeHello(0);
        return;
      }
      document.getElementById('myName').innerHTML = `${myName.substring(0, i + 1)}<span id="typer" aria-hidden="true"></span>`;

      setTimeout(() => {
        typeName(i + 1);
      }, 200);
    }
    typeName(0);
  },
};
</script>
