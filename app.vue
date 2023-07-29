<template>
  <div class="flex h-screen bg-gray-100">
    <div class="m-auto w-11/12 md:w-1/3 space-y-12">
      <div>
        <img
          src="./assets/images/logo-fh-removebg-preview-1.png"
          alt="Logo"
          class="mx-auto"
        />
      </div>
      <div class="space-y-4 text-center capitalize">
        <h1 class="text-4xl font-bold mb-2">Sign In</h1>
        <p class="text-sm text-gray-500">Sistem Informasi Manajemen Keuangan</p>
      </div>
      <div class="bg-white shadow-md rounded-lg p-6">
        <form class="space-y-8">
          <div class="space-y-4">
            <div class="space-y-2">
              <label for="email" class="block text-sm font-medium text-gray-700"
                >Email Address</label
              >
              <input
                type="email"
                id="email"
                class="px-6 py-3 w-full border rounded-full"
                placeholder="angga@yourcomp"
              />
            </div>
            <div class="space-y-2">
              <label
                for="password"
                class="block text-sm font-medium text-gray-700"
                >Password</label
              >
              <input
                type="password"
                id="password"
                class="px-6 py-3 w-full border rounded-full"
                placeholder="*************"
              />
            </div>
          </div>
          <button
            type="submit"
            class="bg-blue-500 text-white px-4 py-2 rounded-full w-full"
          >
            Sign in
          </button>
        </form>
      </div>
    </div>
  </div>
</template>
