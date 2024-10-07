<template>
    <v-container fluid>
      <v-row class="px-6 px-sm-16 flex-column flex-sm-row">
        <v-col cols="12" class="my-12 pa-0">
          <div class="logo">
            <img class="img1" src="/src/assets/logo.svg" alt="" />
          </div>
        </v-col>
        <v-col cols="12" class="d-flex pa-0 mt-6 flex-column flex-sm-row">
          <v-col cols="12" sm="7" class="left pa-0">
            <div>
              <img
                class="img2"
                src="/src/assets/illustration-mockups.svg"
                alt=""
              />
            </div>
          </v-col>
          <v-col cols="12" sm="5" class="right pa-0 px-4">
            <div class="heading">Build The Community Your Fans Will Love</div>
            <div class="para mt-5">
              Huddle re-imagines the way we build communities. You have a voice,
              but so does your audience. Create connections with your users as you
              engage in genuine discussion.
            </div>
            <div class="btn my-5">
              <v-btn
                class="custom-btn text-capitalize d-flex justify-center align-center"
              >
                Register
              </v-btn>
            </div>
          </v-col>
        </v-col>
        <v-col cols="12" class="ml-6 py-0 mt-2">
          <div class="icons">
            <v-col cols="auto" class="icon-wrapper">
              <v-icon icon="mdi-facebook" size="large"></v-icon>
            </v-col>
  
            <!-- Twitter Icon -->
            <v-col cols="auto" class="icon-wrapper ma-0 mx-">
              <v-icon icon="mdi-twitter" size="large"></v-icon>
            </v-col>
  
            <!-- Instagram Icon (Outline) -->
            <v-col cols="auto" class="icon-wrapper">
              <v-icon class="insta" icon="mdi-instagram" size="large"></v-icon>
            </v-col>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <style scoped>
  @font-face {
    font-family: f1;
    src: url(/src/assets/Poppins-SemiBold.ttf);
  }
  @font-face {
    font-family: f2;
    src: url(/src/assets/Poppins-ExtraLight.ttf);
  }
  @font-face {
    font-family: f3;
    src: url(/src/assets/Poppins-Regular.ttf);
  }
  .img1 {
    width: 16%;
  }
  .img2 {
    width: 97%;
  }
  .heading {
    color: white;
    font-size: 35px;
    font-family: f1;
    margin-top: 40px;
  }
  .para {
    color: hsl(260, 100%, 92%);
    font-size: 16px;
    line-height: 23px;
    font-family: f2;
  }
  .custom-btn {
    background-color: white;
    font-family: f3;
    font-size: 16px;
    color: hsl(256, 40%, 49%);
    border-radius: 50px; /* Makes the button capsule-shaped */
    padding: 25px 50px; /* Adjust padding for capsule look */
    text-transform: capitalize; /* Ensures the text is capitalized */
    transition: background-color 0.3s ease, color 0.3s ease; /* Smooth hover transition */
  }
  .icons {
    display: flex;
    justify-content: end;
    font-size: 14px;
  }
  .insta {
    font-size: 24px;
  }
  
  /* Hover effect: pink background and white text */
  .custom-btn:hover {
    background-color: #ff69b4; /* Pink background on hover */
    color: white; /* White text on hover */
  }
  .icon-wrapper {
    --icon-color: #ffffff; /* Default icon color */
    --icon-border-color: #ffffff; /* Default border color */
  
    width: 35px; /* Adjust size as needed */
    height: 35px;
    border: 1px solid var(--icon-border-color); /* Use the custom variable for the border */
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 10px; /* Space between icons */
    transition: border-color 0.3s ease, background-color 0.3s ease, color 0.3s ease;
  }
  
  .icon-wrapper v-icon {
    font-size: 16px;
    color: var(--icon-color); /* Use the custom variable for the icon color */
  }
  
  /* Set unique colors for each icon-wrapper */
  .icon-wrapper:nth-child(1) {
    --icon-color: #ffffff; /* Facebook color */
    --icon-border-color: #ffffff;
  }
  
  .icon-wrapper:nth-child(2) {
    --icon-color: #ffffff; /* Twitter color */
    --icon-border-color: #ffffff;
  }
  
  .icon-wrapper:nth-child(3) {
    --icon-color: #ffffff; /* Instagram color */
    --icon-border-color: #ffffff;
    font-size: 20px;
  }
  
  /* Hover effects */
  .icon-wrapper:hover,
  .icon-wrapper:hover v-icon {
    --icon-color: #ff69b4; /* Pink icon color on hover */
    --icon-border-color: #ff69b4; /* Pink border color on hover */
    color: var(--icon-color); /* Icon color changes on hover */
  }
  
  .icon-wrapper v-icon:hover {
    color: var(--icon-color); /* Ensure icon color changes on hover */
  }
  
  @media screen and (max-width: 599.5px) {
    /* Your CSS rules for screens 599.5px and below */
    .img1 {
      width: 45%;
    }
    .heading {
      margin-top: 100px;
      text-align: center;
      font-size: 30px;
    }
    .para {
      text-align: center;
      padding-left: 40px;
      padding-right: 40px;
      color: white;
    }
    .btn {
      display: flex;
      justify-content: center;
    }
    .icons {
      justify-content: center;
      margin-right: 60px;
      margin-top: 60px;
      margin-bottom: 30px;
    }
  }
  
  @media screen and (min-width: 600px) and (max-width: 959.5px) {
    /* Your CSS rules for screens 959.5px and below */
    .img1 {
      width: 25%;
    }
    .heading {
      font-size: 35px;
      margin-top: 0px;
      font-family: f1;
      line-height: 40px;
    }
    .icons {
      justify-content: center;
      margin-right: 60px;
      margin-top: 30px;
      margin-bottom: 30px;
    }
  }
  </style>
  