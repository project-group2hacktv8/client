<template>
  <div class="home">
     <div class="jumbotron jumbotron-fluid">
        <div class="container">
          <h1 class="display-4">ROCK PAPER SCISSOR classic</h1>
          <p class="lead">This is a modified RPS game with vue and socket.io</p>
        </div>
        <div >
            <img src="https://images-na.ssl-images-amazon.com/images/I/61QkvmvEdVL.png"
            class="rounded mx-auto d-block"
            alt="...">
        </div>
    </div>

    <div class="center-text login">
    <form action="submit">
        <label for="username">User Name</label>
        <input type="username">
        <button class="submit">Go</button>
    </form>
    </div>

    <div v-if="winCondition">You're winning</div>
    <div v-else>You're losing</div>

    <div class="flex">
      <img src="../assets/rock.svg" alt="rock" class="rock">
      <img src="../assets/paper.svg" alt="paper" class="paper">
      <img src="../assets/scissor-tool-with-broken-lines.svg" alt="scissor" class="scissor">
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  data () {
    return {
      winCondition: ''
    }
  }
}
</script>

<style>
body {
    background-image: url("https://image.freepik.com/free-vector/dreamy-soft-clouds-background-with-glowing-sun_1017-23281.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
  }

.rock {
    width:100%;
    height: 230px;
}

.paper {
    width:100%;
    height: 230px;
}

.scissor {
    width:100%;
    height: 230px;
}
</style>
