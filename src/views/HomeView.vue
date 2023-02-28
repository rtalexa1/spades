<template>
  <div class="main-menu">
    <h1 class="game-title">Spades</h1>
    <div class="links">
      <p>Play some damn spades.</p>
      <RouterLink to="/join_game">Join a game</RouterLink>
      <RouterLink to="/host_game">Host a game</RouterLink>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
}
</script>

<style>
.main-menu {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 50px;
  width: 80%;
  min-height: 25em;
}

.game-title {
  -webkit-text-stroke: 5px black;
  color: white;
  font-size: 6em;
}

.links {
  display: flex;
  flex-direction: column;
  align-items: center;
  border-radius: 5px;
  width: 40%;
  height: 10em;
  background-image: linear-gradient(
    0deg,
    hsl(153deg 100% 16%) 0%,
    hsl(145deg 43% 27%) 11%,
    hsl(142deg 28% 36%) 22%,
    hsl(141deg 19% 44%) 33%,
    hsl(140deg 15% 53%) 44%,
    hsl(139deg 15% 62%) 56%,
    hsl(138deg 15% 70%) 67%,
    hsl(138deg 14% 79%) 78%,
    hsl(137deg 13% 88%) 89%,
    hsl(0deg 0% 98%) 100%
  );
  text-align: center;
}
</style>
