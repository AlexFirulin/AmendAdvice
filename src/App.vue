<template>
  <div class="bg-black min-h-screen">
    <div class="header">
      <h1 class="header"><img src="@/assets/images/Logo.png" alt="/" srcset=""></h1>
    </div>

    <div class="container flex flex-col">
      <div class="main flex flex-col">
      <img src="@/assets/images/Frame16.png" alt="My Image" class="mt-28 mr-56">
      <div class="message"> &#x1F32E; &#x2049;😱

</div>
      <img src="@/assets/images/Frame21.png" alt="My Image" class="mt-8 ml-56">
      <div class="answear">🤔💪🤳</div>
    </div>

      <div class="text-container mt-8">
        <span class="text-green">ывфвыфвфывфыыфв</span>
        <h1 class="text-white mt-4 mb-2 font-bold text-3xl md:text-4xl">Instant help with anything</h1>
      </div>

      <button class="mt-10 bg-blue flex items-center justify-center text-white">
        <span class="text-xl font-bold" >NEXT -&gt;</span>
      </button>
    </div>

    <router-view />
  </div>
</template>


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
    background-color: black;
  }


.header {
  height: 375px;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  padding-top:7vh;
}


  .container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    margin-top: -200px;
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
  z-index: 2;
  border-radius: 32px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 8px;
  gap: 10px;
  width: 98px;
  height: 44px;
  position: absolute;
  top: 95px;
  right: 770px;
}
.answear{
  display: flex;
flex-direction: row;
justify-content: center;
align-items: center;
padding: 8px;
gap: 10px;
z-index: 2;

position: absolute;
width: 98px;
height: 44px;
right: 670px;
top: 210px;

background: #99F96C;
border-radius: 32px;
}


  .text-container {
  margin-top: 80px;
  text-align: left;
  display: flex;
  align-self: start;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-left: 30%;

}

  span.text-green {
    color: var(--color-secondary);
  }

  h1 {
    font-size: var(--font-size-large);
    margin-top: 0;
    margin-bottom: 0;
  }

  button {
    width: var(--button-width);
    height: var(--button-height);
    border-radius: var(--button-border-radius);
    background-color: var(--color-primary);
    margin-top: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    border: none;
    position: relative;
    z-index: 1;
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
