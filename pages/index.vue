<template>
  <div>
    <div class="container mt-10">
      <div class="flex">
        <div class="w-1/3 flex justify-center flex-col">
          <h2 class="text-white text-7xl font-smei-bold leading-tight">
            Hire the best development team now
          </h2>
          <h4 class="text-white mt-10 text-xl">
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
      <div class="bg-white rounded-md p-3">
        <div class="hero-btn flex justify-center text-center py-10 rounded-md">
          <p class="text-2xl font-semi-bold w-1/2 text-white">
            We are a team of affordable development experts who save your time
            and resources
          </p>
        </div>
        <div class="py-6">
          <div class="grid grid-cols-4 gap-y-6">
            <div
              v-for="(data, index) in servicesData"
              :key="index"
              class="col-span-1 place-self-center"
            >
              <div class="flex flex-col items-center">
                <div
                  class="
                    border-2 border-blue-500
                    shadow
                    hover:shadow-lg hover:ease-in-out
                    rounded-md
                    flex
                    justify-center
                    items-center
                    p-4
                    w-40
                    h-40
                  "
                >
                  <img
                    class="h-20"
                    :src="require(`@/assets/home/${data.img}`)"
                    alt=""
                  />
                </div>
                <p class="mt-6">{{ data.text }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="py-48 flex">
        <div class="w-1/2 grid grid-cols-2 gap-x-11 gap-y-24">
          <div
            v-for="(data, index) in knowMore"
            :key="index"
            class="col-span-1"
          >
            <div class="rounded-t-md hero-btn h-24 relative">
              <div
                class="
                  absolute
                  rounded-full
                  p-2
                  -top-6
                  left-4
                  bg-blue-400 bg-opacity-40
                "
              >
                <div
                  class="
                    h-16
                    w-16
                    rounded-full
                    bg-white
                    flex
                    justify-center
                    items-center
                  "
                >
                  ABCD
                </div>
              </div>
            </div>

            <div class="bg-white px-4 pt-3 pb-6 rounded-b-md">
              <h3 class="text-2xl">{{ data.heading }}</h3>
              <p class="mt-5 text-sm text-gray-600">
                {{ data.text }}
              </p>
              <button class="mt-5">Know More</button>
            </div>
          </div>
        </div>
        <div class="w-1/2 text-left flex flex-col items-end">
          <h1 class="text-white text-7xl font-semi-bold w-2/3 leading-tight">
            Outsourcing helps you scale faster!
          </h1>
          <p class="mt-8 text-white w-2/3 text-xl">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nobis
            culpa rem temporibus nesciunt deserunt saepe atque illum, libero
            neque quae provident doloribus earum architecto enim animi
            reiciendis est delectus impedit?
          </p>
          <button
            class="
              hero-btn
              text-white text-xl
              px-3
              py-3
              mt-6
              rounded-md
              items-start
            "
          >
            Know More
          </button>
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
      servicesData: [
        {
          text: "Web Development",
          img: "web-development.png",
        },
        {
          text: "UI/UX Design",
          img: "ui-ux-design.png",
        },
        {
          text: "DevOps services",
          img: "devops-services.png",
        },
        {
          text: "Testing services",
          img: "testing-services.png",
        },
        {
          text: "Native App Development",
          img: "native-app-development.png",
        },
        {
          text: "Hybrid App Development",
          img: "hybrid-app-development.png",
        },
        {
          text: "Fixed Scope Projects",
          img: "fixed-scope-projects.png",
        },
        {
          text: "Tech Consulting",
          img: "tech-consulting.png",
        },
      ],
      knowMore: [
        {
          heading: "Code Maintenance",
          text: "Dont't want aggressive development? We can still build products with all essential features by maintaining the code.",
        },
        {
          heading: "Code Maintenance",
          text: "Dont't want aggressive development? We can still build products with all essential features by maintaining the code.",
        },
        {
          heading: "Code Maintenance",
          text: "Dont't want aggressive development? We can still build products with all essential features by maintaining the code.",
        },
        {
          heading: "Code Maintenance",
          text: "Dont't want aggressive development? We can still build products with all essential features by maintaining the code.",
        },
      ],
    };
  },
  mounted() {
    console.log(this.servicesData);
  },
};
</script>
<style lang="scss" >
.hero-btn {
  background: #0575e6;
}
</style>
