<template>
  <div>
    <div class="container mt-10">
      <div class="flex">
        <div class="w-1/3 flex justify-center flex-col">
          <h2 class="text-white text-7xl font-smei-bold">
            Hire the best development team now
          </h2>
          <h4 class="text-white mt-10">
            Kick start and accelerate your software projects with the experts,
            fast deadlines, premium quality coding and no extra fees.
          </h4>
          <div class="mt-8">
            <button class="px-4 py-2 rounded hero-btn">
              <span class="text-white">Let go of your tech worries!</span>
            </button>
          </div>
        </div>
        <div class="w-2/3 flex justify-end">
          <img src="~/assets/home/hero-img.png" alt="" />
        </div>
      </div>
      <div class="py-40">
        <div class="flex justify-between">
          <div
            v-for="(data, index) in heroData"
            :key="index"
            class="hero-btn rounded-md p-5 flex flex-col items-center"
          >
            <p class="text-white text-3xl font-bold">{{ data.number }}</p>
            <span class="text-white text-xl inline-block mt-2">{{
              data.text
            }}</span>
          </div>
        </div>
      </div>
      <div class="bg-white rounded p-2">
        <div class="hero-btn flex justify-center text-center py-10">
          <p class="text-2xl font-semi-bold w-1/2 text-white">
            We are a team of affordable development experts who save your time
            and resources
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      heroData: [
        {
          number: "2019",
          text: "Year Established",
        },
        {
          number: "30+",
          text: "Projects Completed",
        },
        {
          number: "70+",
          text: "Skilled Resources",
        },
        {
          number: "20+",
          text: "Satisfied Customer",
        },
      ],
    };
  },
};
</script>
<style lang="scss" >
.hero-btn {
  background: #0575e6;
}
</style>
