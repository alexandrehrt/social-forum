<script lang="ts">
  import { Input, Label, Helper, Button, Checkbox, A } from 'flowbite-svelte';
  import logo from '$lib/images/logo-2.png';
</script>

<form method="POST" class="p-4 w-screen max-w-md">
  <div class="mb-4 w-100 flex justify-center">
    <img src={logo} alt="logo" class="h-auto w-48 rounded-full" />
  </div>

  <Label class="text-white" for="username">Username</Label>
  <Input name="username" id="username" type="text" placeholder="Username" class="mt-2 mb-4" />

  <Label class="text-white" for="email">Email</Label>
  <Input name="email" id="email" type="email" placeholder="Email" class="mt-2 mb-4" />

  <Label class="text-white" for="password">Password</Label>
  <Input name="password" id="password" type="password" placeholder="Password" class="mt-2 mb-4" />

  <div class="my-2 flex justify-end items-center flex-row-reverse">
    <Label class="text-white" for="remember">Remember me</Label>
    <Checkbox name="remember" id="remember" label="Remember me" />
  </div>

  <div class="w-100 my-4">
    <Button type="submit" class="w-full">Login</Button>
  </div>

  <div class="mt-2">
    <Helper>
      <A href="#">Forgot password?</A>
    </Helper>
  </div>
</form>
