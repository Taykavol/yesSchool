<template>
  <section class="text-gray-700 body-font">
    <div class="flex justify-around items-end mx-5 ">
      <div v-for="(item, index) in items" :key="index" class="flex flex-col items-center w-full  ">
      <div class="flex flex-col justify-center items-center">
        <div class="">
          <h2 class="font-medium title-font text-gray-900 mb-1 text-xl ">
            {{ item.title }}
          </h2>
        </div>
        <p class="leading-relaxed text-center">
          {{ item.text }}
        </p>
      </div>
      <div
        class="flex-shrink-0 w-24 h-24 bg-indigo-100 text-indigo-500 rounded-full inline-flex items-center justify-center"
      >
        <svg
          fill="none"
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          class="w-12 h-12 "
          viewBox="0 0 24 24"
        >
          <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path>
        </svg>
      </div>
    </div>
    </div>
    
    <div class=" px-5 mx-auto flex   ">
      <div
        v-for="(item, index) in items"
        :key="index"
        class="flex flex-col  relative pt-10 pb-10 sm:items-center md:w-2/3 mx-auto"
      >
        <div
          class="h-full w-full absolute inset-0 flex items-center justify-center"
        >
          <div class="h-1 w-full bg-gray-200  "></div>
          <div class="absolute left-0 h-1 w-0 bg-gray-700 stick "></div>
        </div>
        <div
          class=" flex-shrink-0 w-6 h-6 rounded-full mt-10 sm:mt-0 inline-flex items-center justify-center bg-indigo-500 text-white relative z-10 title-font font-medium text-sm"
        >
          {{ item.id }}
        </div>
      </div>
    </div>
  </section>
</template>

<div
  class="flex-grow md:pl-8 pl-6 flex sm:items-center items-start flex-col sm:flex-row"
>
          <div
            class="flex-shrink-0 w-24 h-24 bg-indigo-100 text-indigo-500 rounded-full inline-flex items-center justify-center"
          >
            <svg
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="w-12 h-12 "
              viewBox="0 0 24 24"
            >
              <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path>
            </svg>
          </div>
          <div class=" w-32 sm:pl-6 mt-6 sm:mt-0  absolute text-good">
            <div class="">
              <h2 class="font-medium title-font text-gray-900 mb-1 text-xl ">
                {{ item.title }}
              </h2>
            </div>
            <p class="leading-relaxed">
              {{ item.text }}
            </p>
          </div>
        </div>

<script>
export default {
  data() {
    return {
      items: [
        {
          id: 1,
          svgPath: "",
          title: "Запись на занятие",
          text: "Позвоните нам и мы договоримся обо всем!"
        },
        { id: 2, svgPath: "", title: "Тестирование", text: "Нам важно знать ваш уровень! Тестирование бесплатно" },
        { id: 3, svgPath: "", title: "Обучение", text: "Лучшие педагоги помогут вам выучить иностранный язык!" },
        { id: 4, svgPath: "", title: "Цель достигнута", text: "Ваш иностранный язык стал заметно лучше, может быть advance?" }
      ]
    };
  },
  mounted() {
    window.addEventListener('scroll',()=>{
      if(window.pageYOffset>1300&&window.pageYOffset<1400) {
        console.log('animation was started')
        this.startAnimation()
      }
      
    })
  },
  methods: {
    startAnimation() {
      const element = document.getElementsByClassName("stick");
      console.log(element[0]);
      let i = 0;
      const maxI = this.items.length;
      element[i].className += " w-full";
      function nextStep() {
        setTimeout(() => {
          i++;
          if (i < maxI) {
            element[i].className += " w-full";
            nextStep();
          }
        }, 1000);
      }
      nextStep();
    }
  }
};
</script>

<style lang="scss">
.text-good {
  left: 150px;
}
.rotateMinus90 {
  transform: rotate(-90deg);
}
.rotatePlus90 {
  transform: rotate(90deg);
}
.stick {
  transition: all 1s linear;

  &--1 {
  }
}
</style>
