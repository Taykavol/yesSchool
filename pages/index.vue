<template>
  <div class="">
    <!-- <section class="header--1 relative grid grid-cols-2 ">
      <div
        class="text-white absolute header--1__btn font-serif text-2xl cursor-pointer border-cool   p-1"
      >
        Записаться на занятие!
      </div>
      <div class="flex items-center ">
        <div class="flex flex-col">
          <img src="/unplush/undraw_destinations.svg" class=" h-32" alt="" />
          <div class=" text-2xl text-green-200 text-center font-serif">
            "High results of our students" -Высокие результаты наших учеников
          </div>
        </div>
      </div>
      <div class="flex items-center ">
        <div class="flex flex-col">
          <img src="/unplush/undraw_exams.svg" class=" h-32" alt="" />
          <div class=" text-2xl text-green-200 text-center font-serif">
            "Passing internationals exams like TOFI,IMD" - Мы готовим к
            международным сдачам экзамена.
          </div>
        </div>
      </div>
      <div class="flex items-center ">
        <div class="flex flex-col">
          <img src="/unplush/undraw_online_test.svg" class=" h-32" alt="" />
          <div class=" text-2xl text-green-200 text-center font-serif">
            "High results of our students" -Высокие результаты наших учеников
          </div>
        </div>
      </div>
      <div class="flex items-center ">
        <div class="flex flex-col">
          <img src="/unplush/undraw_destinations.svg" class=" h-32" alt="" />
          <div class=" text-2xl text-green-200 text-center font-serif">
            "High results of our students" -Высокие результаты наших учеников
          </div>
        </div>
      </div>
    </section> -->
    <section class="header ">
      <div class="nav justify-between flex-col flex ">
        <div class=" flex justify-around">
            <img src="/yes.svg" class="nav__image h-48 -ml-16 " alt="" />
          <div class="uppercase flex  text-3xl text-green-700 ">
            <div class="flex flex-col justify-center text-4xl">
              <div class=" text-center tracking-widest ">Welcome to yeschool!</div>
              <div
                class=" animate__animated animate__pulse  rounded-full px-4 border-black mt-2 border-2 cursor-pointer btn-cta"
              >
                Записаться на занятие
              </div>
            </div>
          </div>
          <div class="flex flex-col self-center">
            <div class="phone self-center text-4xl text-black flex"><img src="/icons/phone-volume-solid.svg" class="h-8 w-8 self-center" alt=""><div class="ml-1" @click="copy">8-8202-622-880</div></div>

            <div class=" flex  justify-center mt-1 ">
              <div class="">
                <img
                  src="/icons/insta.svg"
                  class="icon icon--insta h-12 w-12 "
                  alt=""
                />
              </div>
              <div class="">
                <img
                  src="/icons/vk.svg"
                  class="icon icon--vk h-12 w-12 ml-4 "
                  alt=""
                />
              </div>
              <div class="">
                <img
                  src="/icons/fb.svg"
                  class="icon icon--vk h-12 w-12 ml-4 "
                  alt=""
                />
              </div>
              <div class="">
                <img
                  src="/icons/youtube.svg"
                  class="icon icon--vk h-12 w-12 ml-4 "
                  alt=""
                />
              </div>
              <div class="">
                <img
                  src="/icons/gmail.svg"
                  class="icon icon--vk h-12 w-12 ml-4 "
                  alt=""
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <nav class="nav__box  justify-around md:mx-12 hidden lg:flex sticky top-0">
      <div class="nav__item nav__item--1   ">О нас</div>
      <div class="nav__item nav__item--2  ">Педагоги</div>
      <div class="nav__item nav__item--3   ">Стоимость Обучения</div>
      <div class="nav__item nav__item--4 ">Наши мероприятия</div>
      <div class="nav__item nav__item--4 ">Контакты</div>
    </nav>
    <section class="news__galary">
      <Gallery class=" mx-0 md:mx-24 sm:mx-12 my-12  " />
    </section>
    
    <section class="langs mb-8">
      <div class="langs__title text-center text-3xl font-bold">
        Выбирете язык
      </div>
      <div class="flex justify-center">
        <div class="break"></div>
      </div>
      <div class=""></div>
      <Tabs />
    </section>
    <section class="steps">
      <div class="langs__title text-center text-3xl font-bold">
        Как начать заниматься?
      </div>
      <div class="flex justify-center">
        <div class="break"></div>
      </div>
      <Steps/>
    </section>
    <section class="order"></section>
    <section class="teachers">
      <div class="langs__title text-center text-3xl font-bold">
        Педагоги нашей школы
      </div>
      <div class="flex justify-center">
        <div class="break"></div>
      </div>
      <div class="flex justify-around flex-wrap ">
        <CardTeachers />
        <CardTeachers />
        <CardTeachers />
        <CardTeachers />
        <CardTeachers />
        <CardTeachers />
      </div>
    </section>
  </div>
</template>

<script>
import CardTeachers from "@/components/CardTeacher";
import Gallery from "@/components/Gallery";
import Tabs from "@/components/Tabs";
import Steps from "@/components/Steps"
import 'animate.css'
export default {
  components: {
    Gallery,
    Tabs,
    CardTeachers,
    Steps
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap");

/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.header--1 {
  &__btn {
    top: 20vh;
    left: 50%;
    background-image: linear-gradient(90deg, silver 50%, transparent 50%),
      linear-gradient(90deg, silver 50%, transparent 50%),
      linear-gradient(0deg, silver 50%, transparent 50%),
      linear-gradient(0deg, silver 50%, transparent 50%);
    background-repeat: repeat-x, repeat-x, repeat-y, repeat-y;
    background-size: 15px 2px, 15px 2px, 2px 15px, 2px 15px;
    background-position: left top, right bottom, left bottom, right top;
    animation: border-dance 1s infinite linear;
    transform: translate(-50%, -50%);
    padding: 5px;
  }
  column-gap: 45rem;
  height: 110vh;
  background: url("/yes.svg") center -20px no-repeat,
    radial-gradient(
      37.86% 77.79% at 50% 100%,
      rgba(113, 128, 150, 0.25) 0%,
      rgba(113, 128, 150, 0) 100%
    ),
    linear-gradient(180deg, #1a202c 0%, #2d3748 100%),
    linear-gradient(180deg, #0d0f14 0%, rgba(27, 32, 43, 0) 100%), #2f3747;
}
.break {
  margin-top: 1rem;
  margin-bottom: 4rem;
  width: 100px;
  border-bottom: 2px solid black;
}
.header {
  font-family: "Oswald", sans-serif;
}
.icon {
  cursor: pointer;
  &--insta {
    transition: transform 0.5s;
    &:hover {
      transform: scale(1.3) rotate(360deg);
    }
  }
  &--vk {
    transition: transform 0.5s;
    &:hover {
      transform: scale(1.3);
    }
  }
}
.nav {
  &__box {
    z-index: 20;
    background-color: white;
  }
  &__item {
    padding: 0.5rem;
    font-weight: 300;
    text-align: center;
    font-weight: bold;
    // border-radius: 0.3rem;
    font-size: 1.6rem;
    // border-bottom: 2px solid black;
    cursor: pointer;
    &:hover {
      @apply bg-gray-200;
    }

    // @apply text-green-500 text-2xl font-serif font-bold;
    // &--1 {
    //   top: 8rem;
    //   left: 8rem;
    // }
    // &--2 {
    //   top: 8rem;
    //   right: 8rem;
    // }
    // &--3 {
    //   bottom: 8rem;
    //   left: 8rem;
    // }
    // &--4 {
    //   bottom: 8rem;
    //   right: 8rem;
    // }
  }
  &__image {
  }
  .border-cool {
  }
  .btn-cta {
    animation-iteration-count: 100;
  }
  @keyframes border-dance {
    0% {
      background-position: left top, right bottom, left bottom, right top;
    }
    100% {
      background-position: left 15px top, right 15px bottom, left bottom 15px,
        right top 15px;
    }
  }
}
</style>
