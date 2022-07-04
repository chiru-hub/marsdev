<template>
  <div>
    <div class="border border-white"></div>
    <div class="container">
      <div class="flex my-16">
        <div class="w-1/3">
          <div class="flex">
            <div>
              <img src="~/assets/pointer-usa.png" alt="" />
            </div>
            <div class="text-white ml-4">
              <p class="text-3xl">USA:</p>
              <p class="text-xl mt-2">
                3422, Old Capitol Trail, Suite 93, <br />Wilmington, DE 1980<br />
                Phone: +1 4422615154
              </p>
            </div>
          </div>
          <div class="flex mt-16">
            <div>
              <img src="~/assets/pointer-india.png" alt="" />
            </div>
            <div class="text-white ml-4">
              <p class="text-3xl">USA:</p>
              <p class="text-xl mt-2">
                SN 71/8/2, Jijai Nagar, Kothrud, <br />
                Pune 411038 <br />
                Phone:+91 9322358095
              </p>
            </div>
          </div>
        </div>
        <div class="w-1/3 flex flex-col items-center">
          <div>
            <div class="text-white">
              <p class="opacity-60 text-4xl">Quick Links</p>
              <div class="mt-2">
                <nuxt-link class="block text-xl text-left mt-2" to=""
                  >Contact</nuxt-link
                >
                <nuxt-link class="block text-xl text-left mt-2" to=""
                  >Blog</nuxt-link
                >
                <nuxt-link class="block text-xl text-left mt-2" to=""
                  >Careers</nuxt-link
                >
              </div>
            </div>
            <div class="text-white mt-8">
              <p class="opacity-60 text-4xl">Legal</p>
              <div class="mt-2">
                <nuxt-link class="block text-xl text-left mt-2" to=""
                  >Privacy Policy</nuxt-link
                >
              </div>
            </div>
          </div>
        </div>
        <div class="w-1/3 flex justify-center">
          <div>
            <div>
              <img src="~/assets/logo.png" alt="" />
            </div>
            <div class="mt-8 text-white">
              <p class="text-4xl">Follow Us:</p>
              <div class="flex mt-8">
                <img class="mr-7" src="~/assets/instagram.png" alt="" />
                <img class="mr-7" src="~/assets/facebook.png" alt="" />
                <img class="mr-7" src="~/assets/twitter.png" alt="" />
                <img src="~/assets/linkedin.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="border border-white"></div>
    <div class="container">
      <div class="flex mt-5 mb-10 justify-around">
        <div class="w-1/3"></div>
        <div class="w-1/3">
          <p class="text-white text-center">
            © 2005-2022 Marsdevs, All rights reserved
          </p>
        </div>
        <div class="w-1/3">
          <div class="flex justify-end">
            <img src="~/assets/double-left.png" alt="" />
            <img class="ml-3" src="~/assets/double-up.png" alt="" />
            <img class="ml-3" src="~/assets/footer-home.png" alt="" />
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
</style>
