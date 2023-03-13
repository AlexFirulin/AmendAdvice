<template>
  <div class="bg-black screen">
  <div class="create">
    <span class="amend-acc">Your amend account</span>
  </div>
  <div>
    <span class="loggin">Login with your phone number</span>
  </div>
  <div class="inputs bg-black text-white">
    <input type="number" class="code"> <input type="tel" class="phone">
  </div>
  <div class="bg-black text-white msg-send">
    We will send verification code to this number
  </div>
  <div class="cont">
    <button class="btn-cont">Continue</button>
  </div>
  <div class="bg-black text-white flex acces links">
    <a href=""><p>Changed phone number?</p></a>
    <a href=""><p>Restore access</p></a>
  </div>
</div>
<router-view />
</template>





<style>
.screen{
  max-height: 100vh;
  min-height: 100vh;
  min-width: 100vw;
}
.amend-acc{
font-family: 'Inter';
font-style: normal;
font-weight: 600;
font-size: 16px;
line-height: 24px;
display: flex;
align-content: center;
text-align: center;
justify-content: center;
color: #15FE02;
}

.create{
padding-top:10vh ;
letter-spacing: -0.02em;
background: black;
order: 0;
flex-grow: 0;
}

.loggin{
color: white;
width: 100%;
height: 10vw;

font-family: 'Inter';
font-style: normal;
font-weight: 600;
font-size: 32px;
line-height: 125%;
/* or 40px */

letter-spacing: -0.02em;

/* Neutral/White */

color: #FFFFFF;
background: black;


/* Inside auto layout */
display: flex;
justify-content: center;
text-align: center;
position: inherit;
}

.inputs{
/* Inside auto layout */
display: flex;
justify-content: center;
gap: 8px;
color: black;
}
.code{
  border: 0.5px solid #333333;
border-radius: 8px;
}
.msg-send{
font-family: 'Inter';
font-style: normal;
font-weight: 400;
font-size: 16px;
line-height: 22px;
/* identical to box height, or 138% */

letter-spacing: -0.02em;

/* Neutral/Lightest */

color: #BEBEBE;
display: flex;
justify-content: center;
}

.cont{
  display: flex;
  align-items: center;
  background-color: black;
  justify-content: center;
  margin-top: 10vh;
}
.btn-cont{
display: flex;
justify-content: center;
align-items: center;
gap: 8px;
width: 343px;
height: 54px;
/* Brand/Primary */
background: #5843F4;
border-radius: 16px;
}
.links{


font-family: 'Inter';
font-style: normal;
font-weight: 400;
font-size: 16px;
line-height: 22px;
/* or 138% */

text-align: center;
justify-content: center;
flex-direction: column;
letter-spacing: -0.02em;
padding-top: 5vh;
}



</style>

