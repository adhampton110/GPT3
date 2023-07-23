<template>
    <header>
    <img src="../../assets/logo.svg" alt="logo">
    <div class="links">
      <a href="#">Home</a>
      <a href="#">What is GPT?</a>
      <a href="#">Open AI</a>
      <a href="#">Case Studies</a>
      <a href="#">Library</a>
    </div>
    <div class="login">
      <a href="#">Sign in</a>
      <button>Sign up</button>
    </div>
  </header>
</template>

<style scoped>
  header {
  padding-top: 55px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

a {
  text-decoration: none;
  color: #FFFFFF;
  font-weight: 400;
}

button {
  width: 152px;
  height: 58px;
  font-size: 18px;
  color: #FFFFFF;
  background-color: rgba(255, 72, 32, 1);
  border-radius: 8px;
  border: none;
}

.links {
  display: flex;
  gap: 30px;
}


.login {
  display: flex;
  gap: 23px;
  align-items: center;
}
</style>