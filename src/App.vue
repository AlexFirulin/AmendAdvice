<template>
  <div class="bg-black min-h-screen max-h-screen">
    <div class="header">
      <img src="@/assets/images/Logo.png" alt="/" srcset="">
    </div>

    <div class="container flex flex-col">
      <div class="main flex flex-col">
        <img src="@/assets/images/Frame16.png" alt="My Image" class="mt-10 md:mt-28 mr-4 md:mr-56">
        <div class="message"> &#x1F32E; &#x2049;😱 </div>
        <img src="@/assets/images/Frame21.png" alt="My Image" class="mt-2 md:mt-8 ml-4 md:ml-56">
        <div class="answear">🤔💪🤳</div>
      </div>

      <div class="text-container mt-2 md:mt-8">
        <span class="text-green">Help on demand</span>
        <h1 class="text-white mt-2 md:mt-4 mb-2 font-bold text-2xl md:text-4xl">Instant help with anything</h1>
      </div>

    <router-link to="LoginPage">
    <div class="flex justify-center mt-5 bg-black">

    <button class="btn  text-white">

  <span class="text-xl font-bold">NEXT-&gt;</span>
      </button>
    </div>
    </router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
</script>


<style lang="scss">
  :root {
    --color-primary: #5843F4;
    --color-secondary: #15FE02;
    --font-size-large: 32px;
    --font-size-medium: 20px;
    --button-width: 295px;
    --button-height: 60px;
    --button-border-radius: 16px;
  }

  .bg-black {
    width: auto;
    background-color: black;
    height: auto;
  }

  .header {
    box-sizing: border-box;
    height: 20vw;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    padding-top: 3vh;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    margin-top: -220px;
    position: relative;
    z-index: 1;
  }

  img {
    max-width: 100%;
    height: auto;
    background-color: black;
  }

  .message {
    background-color: yellow;
    border-radius: 32px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 8px;
    gap: 10px;
    width: 98px;
    height: 44px;
    position: relative;
    top: -85px;
    right: -55px;
    z-index: 2;
  }

  .answear {
    background: #99F96C;
    border-radius: 32px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 8px;
    gap: 10px;
    width: 98px;
    height: 44px;
    position: relative;
    right: -160px;
    top: -90px;
    z-index: 2;
  }

  .text-container {
  display: flex;
  flex-direction: column;
}

  span.text-green {
    color: var(--color-secondary);
    display: flex;
  }

  h1 {
    font-size: var(--font-size-large);
    display: flex;
    position: relative;
    top: 1px;
  }


  .btn {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 16px 8px;
  background-color: #5843F4;
  gap: 10px;
  border-radius: 150vh;
  z-index: 1;
  border-radius: 16px;
  position: absolute;
width: 295px;
height: 60px;
}



  button span {
    font-size: var(--font-size-medium);
    color: white;
  }

  @media (max-width: 640px) {
    .header {
      height: 200px;
    }

    h1 {
      font-size: var(--font-size-medium);
    }

    .container {
      margin-top: -150px;
    }

    img {
      margin-top: -100px;
    }

    .text-container {
      margin-top: 50px;
    }

    button {
      width: 100%;
      max-width: var(--button-width);
      margin-top: 30px;
    }
  }
</style>