<template>
    <div class="hello">
        <h1>Public</h1>

        <div id="app">
            {{ msg }}
        </div>

        <h2>Todos</h2>
        <ul>
            <li>Konten</li>
            <li>Private</li>
            <li>Events</li>
        </ul>
    </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

