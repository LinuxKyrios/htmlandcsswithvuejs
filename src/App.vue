<template>
  <div id="app" >
    <h4 class="bg-success text-dark text-center m-1 p-2">
      Technology stack that Linux Kyrios wish to master
    </h4>
    <table class="table table-striped table-bordered table-sm">
      <thead>
      <tr><th>Technology stack</th><th>Does Linux Kyrios know this stack?</th></tr>
      </thead>
      <tbody>
        <tr v-for="s in stack" v-bind:key="s.action">
          <td>{{s.action}}</td>
          <td>{{s.done}}</td>
        </tr>
      </tbody>
    </table>
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
