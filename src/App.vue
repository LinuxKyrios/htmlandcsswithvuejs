<template>
  <div id="app">
    <h4 class="bg-success text-dark text-center p-2">
      Technology stack that Linux Kyrios wish to master
    </h4>
    <div class="container-fluid p-4">
      <div class="row">
        <div class="col font-weight-bold">Technology stack</div>
        <div class="col-2 font-weight-bold">Does Linux Kyrios know this stack?</div>
      </div>
      <div class="row" v-for="s in stack" v-bind:key="s.action">
        <div class="col">{{s.action}}</div>
        <div class="col-2">{{s.done}}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  //name: 'App',
  data: function() {
    return {
      stack: [{ action: "JavasScript", done: true },
              { action: "Vue.js", done: false },
              { action: "React", done: false },
              { action: "Angular", done: false },
              { action: ".NET Core MVC", done: false },
              { action: "C#", done: false }]
    }
  }
}
</script>
