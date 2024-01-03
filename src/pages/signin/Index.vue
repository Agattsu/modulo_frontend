<template>
  <q-page class="flex flex-center column">
    <q-img src='../../../src/assets/modelofrontend-logo.svg' ></q-img>
    <q-input filled v-model="text" label='Filled' />
    <q-input filled v-model="text" label='Filled' />
    <a href="">Forgot password?</a>
    <q-btn color="primary" label="Log In" />
    <div class="flex row" >
      <q-img src="../../../src/assets/facebook-logo.svg" ></q-img>
      <a href="">Log in with Facebook</a>
    </div>
    <div class= "full-width">
       <q-separator />
       or
        <q-separator />
    </div>
    <div>
      Don't have an account? <a href="">Sign up.</a>
    </div>
    <q-separator />
    Instagram or Facebook
  </q-page>
</template>

<script>
export default {
  name: 'SignIn',
  data() {
    return {
      text: '',
    };
  },
};
</script>
