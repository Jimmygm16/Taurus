<script setup></script>

<template>
  <main class="main-content">
    <img class="taurus" src="../assets/images/taurus.jpg" alt="taurus image" />
    <div class="taurus-options">
      <span class="taurus-greet">Hello I'm Taurus, what do you want to do?</span>
    </div>
  </main>
</template>

<style scoped>
.main-content {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  background-color: #1a1a1a;
  color: white;
}

.taurus {
  width: 100%;
  height: 100%;
}

.taurus-greet {
  font-size: 2rem;
  font-weight: 800;
  color: var(--title_color);
  text-align: center;
}

.taurus-options {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 5rem;
  border-left: solid 0.5rem var(--title_color);
}
</style>
