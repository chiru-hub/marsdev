<template>
  <div>
    <div class="container mt-10">
      <div class="flex">
        <div class="w-1/3 flex justify-center flex-col">
          <h2 class="text-white text-7xl font-semi-bold leading-tight">
            Lets learn together!!
          </h2>
          <h4 class="text-white mt-10 text-xl">
            We solve tech issues. But, you need to identify them!, So we present
            with you resources that help you understand development better so
            you can let us know whats's wrong.
          </h4>
          <div class="mt-8">
            <button class="px-4 py-2 rounded color-secondary">
              <span class="text-white">Know more</span>
            </button>
          </div>
        </div>
        <div class="w-2/3 flex justify-center">
          <img class="w-full" src="~/assets/blog/hero-img-blog.png" alt="" />
        </div>
      </div>
      <div class="my-48">
        <p class="text-white text-7xl font-semi-bold">Blogs</p>
        <div class="pt-40">
          <div
            v-for="(data, index) in 7"
            :key="index"
            class="color-secondary p-10 rounded-lg mb-20"
          >
            <div class="grid grid-cols-3 p-3 gap-x-20">
              <div
                v-for="(data, index) in 3"
                :key="index"
                class="col-span-1 rounded-lg bg-white p-5"
              >
                <nuxt-link to="/blogs/hello">
                  <img
                    class="flex justify-center"
                    src="~/assets/blog/Mask-29.png"
                    alt=""
                  />
                  <p class="text-sm mt-4">
                    Should we reshape your talent sourcing strategy?
                  </p>
                  <div class="mt-3 flex justify-end">
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="h-6 w-6"
                      fill="none"
                      viewBox="0 0 24 24"
                      stroke="currentColor"
                      stroke-width="2"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        d="M14 5l7 7m0 0l-7 7m7-7H3"
                      />
                    </svg>
                  </div>
                </nuxt-link>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.color-secondary {
  background: #0575e6;
}
</style>
