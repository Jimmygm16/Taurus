<script setup>
import { useRouter } from 'vue-router'

const router = useRouter()
</script>

<template>
  <main class="home-content">
    <div class="title-content">
      <span></span>
      <h1 class="title">Taurus Code Manager</h1>
      <button
        @click="
          () => {
            router.push('/taurus')
          }
        "
        class="btn-start"
      >
        start
      </button>
    </div>
    <section class="information">
      <p class="about-taurus">
        Taurus Code Manager is an assistant for your projects that uses the OpenAI API. It helps you
        from the beginning to the end of your project. You can ask about what tecnologies to use,
        how to implement a feature, how to deploy your project, etc. Once you have clear how should
        your project be, you can even ask Taurus to check your code and give you some feedback.
      </p>
      <img class="icon" src="../assets/icon/openai.svg" alt="openai icon" fill="#F28B0C" />
    </section>
  </main>
</template>

<style scoped>
.home-content {
  width: 100%;
  height: 100vh;
  color: white;
  background-color: #212121;
}

.title-content {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-content: center;
  align-items: center;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.3rem;
  text-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  padding: 2rem;
  background-color: rgb(0, 0, 0, 0.2);
  color: var(--title_color);
}

.title {
  display: flex;
  text-align: center;
}

.information {
  display: flex;
  flex-direction: column;
  gap: 3rem;
  justify-content: center;
  align-items: center;
}

.about-taurus {
  display: flex;
  justify-self: center;
  padding: 2rem;
  font-size: 1.5rem;
  line-height: 2rem;
  text-align: center;
  text-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  border-bottom: solid 0.3rem var(--title_color);
  width: 60%;
}

.btn-start {
  justify-self: center;
  padding: 0.5rem 2.5rem;
  font-size: 1.5rem;
  font-weight: 800;
  background-color: var(--title_color);
  color: white;
  border: none;
  border-radius: 0.5rem;
  cursor: pointer;
  transition: all 0.3s;
}

.btn-start:hover {
  transform: scale(1.1);
}
.icon {
  width: 8rem;
  height: 8rem;
  filter: drop-shadow(0 0 10px rgba(0, 0, 0, 0.5));
}
</style>
