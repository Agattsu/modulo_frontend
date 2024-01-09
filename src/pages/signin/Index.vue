<template>
  <q-page class="flex flex-center column justify-center q-px-md">

    <div class="full-width column items-center justify-center">
    <q-icon name="fas fa-chevron-left"
    size="18px"
    color="grey"
    class="absolute-left q-ma-lg"></q-icon>
    <q-img class="logo q-mb-lg" src='../../../src/assets/modelofrontend-logo.svg' ></q-img>
    <q-input filled v-model="email" label='E-mail' class='full-width q-mb-md' />
    <q-input filled v-model="password" label='Password' type="password" class='full-width' />

    <div class= "column items-end full-width">
    <a class="q-mt-md link" href="">Forgot password?</a>
    </div>

    <q-btn color="primary" label="Log In" class="sign-in-button full-width q-mt-lg" />

    <div class="flex full-width row items-center justify-center q-mt-xl" >
      <q-img class="facebook-icon" src="../../../src/assets/facebook-logo.svg" ></q-img>
      <a href="" class="link q-ml-xs">Log in with Facebook</a>
    </div>

    <div class= "full-width row items-center justify-center q-my-xl">
       <q-separator class="separator" inset />
       OR
        <q-separator class="separator" inset />
    </div>

    <div class="full-width row items-center justify-center">
      Don't have an account? <a href="" class="link q-ml-xs">Sign up.</a>
    </div>
    </div>
    <div class="full-width column items-center absolute-bottom">
      <q-separator class="full-width"/>
    <div class="q-my-lg">
      <span class="text-black-opacity">Instagram or Facebook</span>
    </div>
    </div>
  </q-page>

</template>

<script>
export default {
  name: 'SignIn',
  data() {
    return {
      email: '',
      password: '',
    };
  },
};
</script>

<style lang="scss" scoped>
.logo {
  height: 60px;
  width: 182px;
}
.sign-in-button{
  height: 44px;
  border-radius: 5px;
  background-color: #3797EF;
}
.facebook-icon{
  height: 17px;
  width: 17px;
}
.separator {
  width: 35%;
}
</style>
