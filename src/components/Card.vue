<template>
  <form class="card-form">
    <div class="back">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="13"
        height="8"
        viewBox="0 0 13 8"
        fill="none"
      >
        <path
          d="M0.646446 3.64645C0.451184 3.84171 0.451184 4.15829 0.646446 4.35355L3.82843 7.53553C4.02369 7.7308 4.34027 7.7308 4.53553 7.53553C4.7308 7.34027 4.7308 7.02369 4.53553 6.82843L1.70711 4L4.53553 1.17157C4.7308 0.976311 4.7308 0.659728 4.53553 0.464466C4.34027 0.269204 4.02369 0.269204 3.82843 0.464466L0.646446 3.64645ZM13 3.5L1 3.5V4.5L13 4.5V3.5Z"
          fill="black"
        />
      </svg>
      back
    </div>
    <div class="main-content">
      <div class="title">
        <h2 class="sub-title">Start from free</h2>
        <h1 class="title">Create an account</h1>
      </div>
      <div class="sing-up-method d-flex justify-content-between">
        <button class="btn">
          <div class="icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="22"
              height="22"
              viewBox="0 0 22 22"
              fill="currentColor"
            >
              <path
                d="M11 8.8V13.2H17.2238C16.3152 15.7608 13.8688 17.6 11 17.6C7.3612 17.6 4.4 14.6388 4.4 11C4.4 7.3612 7.3612 4.4 11 4.4C12.5774 4.4 14.0954 4.9654 15.2746 5.9928L18.1654 2.6752C16.1854 0.9504 13.6422 0 11 0C4.9346 0 0 4.9346 0 11C0 17.0654 4.9346 22 11 22C17.0654 22 22 17.0654 22 11V8.8H11Z"
              />
            </svg>
          </div>
          Sign up with Google
        </button>
        <button class="btn">
          <div class="icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="12"
              height="22"
              viewBox="0 0 12 22"
              fill="currentColor"
            >
              <path
                d="M9.66391 3.65291H11.6723V0.154909C11.3258 0.107242 10.1342 -7.62939e-06 8.74633 -7.62939e-06C5.85058 -7.62939e-06 3.86692 1.82141 3.86692 5.16908V8.24999H0.671416V12.1605H3.86692V22H7.78475V12.1614H10.851L11.3377 8.25091H7.78383V5.55683C7.78475 4.42658 8.08908 3.65291 9.66391 3.65291Z"
              />
            </svg>
          </div>
          Sign up with Facebook
        </button>
      </div>
      <div class="divider">
        <p>Or use your email for registration</p>
        <div class="line"></div>
      </div>
      <input
        class="firstName"
        type="text"
        name="firstName"
        placeholder="First Name"
        v-model="firstName"
      />
      <input
        type="text"
        class="lastName"
        name="lastName"
        placeholder="Last Name"
        v-model="lastName"
      />
      <input
        type="email"
        name="email"
        placeholder="Email"
        v-model="email"
        class="email"
      />
      <input
        class="password"
        type="password"
        name="password"
        placeholder="Password"
        v-model="password"
      />
      <div class="alert d-flex">
        <div class="characters-min d-flex align-items-center">
          <div class="alert-icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="11"
              viewBox="0 0 11 11"
              fill="currentColor"
            >
              <circle cx="5.5" cy="5.5" r="5.5" fill="currentColor" />
              <path
                d="M3 6.18182L5.08333 8L8 4"
                stroke="white"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <p>8 Characters min.</p>
        </div>
        <div class="one-number d-flex align-items-center ml-4">
          <div class="alert-icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="11"
              height="11"
              viewBox="0 0 11 11"
              fill="currentColor"
            >
              <circle cx="5.5" cy="5.5" r="5.5" fill="currentColor" />
              <path
                d="M3 6.18182L5.08333 8L8 4"
                stroke="white"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <p>One number</p>
        </div>
      </div>
      <div class="policy-check d-flex align-items-center">
        <input type="checkbox" name="policy" id="policy" v-model="check" />
        <label for="policy"
          >By creating account, you agree to accept our Privacy Policy, Terms of
          Service and Notification settings.</label
        >
      </div>
      <button type="submit" class="btn submit">Create an Free Account!</button>
      <p class="login">
        Already have an account?
        <a href="#">Log in</a>
      </p>
    </div>
  </form>
</template>

<script>
export default {
  name: "Card",
  data() {
    return {
      firstName: "",
      lastName: "",
      email: "",
      password: "",
      check: false,
    };
  },
};
</script>

