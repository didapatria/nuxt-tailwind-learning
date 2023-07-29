<template>
  <div class="flex h-screen bg-gray-100">
    <div class="m-auto w-1/3">
      <div class="mb-6">
        <img
          src="./assets/images/logo-fh-removebg-preview-1.png"
          alt="Logo"
          class="mx-auto"
        />
      </div>
      <h1 class="text-2xl font-bold mb-2 text-center capitalize my-6">
        Sign In
      </h1>
      <p class="text-sm text-gray-500 text-center mb-6">
        Sistem Informasi Manajemen Keuangan
      </p>
      <div class="bg-white shadow-md rounded-lg p-8 my-6">
        <form>
          <div class="mb-4">
            <label
              for="email"
              class="block text-sm font-medium text-gray-700 my-2"
              >Email Address</label
            >
            <input
              type="email"
              id="email"
              class="mt-1 px-4 py-2 w-full border rounded-full"
              placeholder="angga@yourcomp"
            />
          </div>
          <div class="mb-4">
            <label
              for="password"
              class="block text-sm font-medium text-gray-700 my-2"
              >Password</label
            >
            <input
              type="password"
              id="password"
              class="mt-1 px-4 py-2 w-full border rounded-full"
              placeholder="*************"
            />
          </div>
          <button
            type="submit"
            class="bg-blue-500 text-white px-4 py-2 rounded-full w-full my-2"
          >
            Sign in
          </button>
        </form>
      </div>
    </div>
  </div>
</template>
