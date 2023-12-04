
import { RouterLink } from 'vue-router';
<template>
  <div class="max-w-7xl mx-auto grid grid-cols-2 gap-4">
    <div class="main-left">
      <div class="p-12 bg-white border border-gray-200 rounded-lg">
        <h1 class="mb-6 text-2xl">Log in</h1>
        <p class="mb-6 text-gray-500">
          Log in to stay connected with your loved once or meet new people!!!
        </p>
        <p class="font-bold">Don't have an account? <RouterLink :to="{'name':'Signup'}" class="underline">Click Here</RouterLink> to create one!
        </p>
      </div>
    </div>

    <div class="main-right">
      <div class="p-12 bg-white border border-gray-200 rounded-lg">
        <form class="space-y-6">
          <div>
            <label>E-mail</label><br>
            <input type="email" placeholder="Enter Your Email address" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" required>
          </div>

          <div>
            <label>Password</label><br>
            <input type="password" placeholder="Enter Password" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" required>
          </div>

          <div>
            <button class="py-4 px-6 bg-purple-600 text-white rounded-lg">Log in</button>
          </div>

        </form>
      </div>
    </div>

  </div>
</template>