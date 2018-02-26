<template>
  <div id="app">
    <Room id="room"></Room>
    <UserList id="user-list"></UserList>
    <Cards id="cards"></Cards>
  </div>
</template>

<script>
  import Cards from './components/Cards';
  import Room from './components/Room';
  import UserList from './components/UserList';

  export default {
    name: 'app',
    components: {
      Cards,
      Room,
      UserList
    },
    data() {
      return {
        users: [],
        cards: [],
        room: {
          name: 'example'
        }
      }
    }
  }
</script>

<style lang="scss">
  html {
    box-sizing: border-box;
  }

  *, *:before, *:after {
    box-sizing: inherit;
  }

  body {
    margin: 0;
  }

  #room {
    background: red;
    color: white;
  }

  #user-list {
    background: blue;
    color: white;
  }

  #cards {
    background: green;
    color: white;
  }

  #app {

  }
</style>
