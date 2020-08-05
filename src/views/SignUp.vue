<template>
  <div class="signup">
    <h2>SignUp</h2>
    <form>
      <label class="form3" for="name">Name</label>
      <input
        aria-invalid="false"
        autocomplete="name"
        id="name"
        name="name"
        required
        type="text"
        value
      />

      <label class="form4" for="email">Email Address</label>
      <input
        aria-invalid="false"
        autocomplete="email"
        id="email"
        name="email"
        required
        type="text"
        value
      />

      <label class="form5" for="Password">Password</label>
      <input
        aria-invalid="false"
        autocomplete="password"
        id="password"
        name="password"
        required
        type="text"
        value
      />

      <label class="form6" for="confirmPassword">ConfirmPassword</label>
      <input
        aria-invalid="false"
        autocomplete="confirmpassword"
        id="confirmpassword"
        name="confirmpassword"
        required
        type="text"
        value
      />
      <button type="sumbit">
        <span class="btn"></span>Sign in
      </button>
    </form>
  </div>
</template>