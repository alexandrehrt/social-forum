<script lang="ts">
  import LoginForm from '../components/Forms/login/login-form.svelte';
  import backgroundImage from '$lib/images/logo.png';
</script>

<div class="bg-background min-h-screen h-full flex justify-center items-center md:justify-">
  <div id="bg-div" class="hidden md:block">
    <img src={backgroundImage} alt="background" class="md:h-screen md:w-100" />
  </div>

  <LoginForm />
</div>
