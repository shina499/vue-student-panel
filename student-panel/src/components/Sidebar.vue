<script setup>
import { ref } from 'vue';

const menuItems = [
  { path: '/', name: "داشبورد دانش آموزی📚🖋️", bgClass: "bg-red-200", buttonClass: "bg-red-500",shadowColor:"shadow-red-500" , buttonHover: "hover:bg-red-600", buttonText: "پیش به سوی آن!" },
  { path: '/exam', name: "پنل امتحانات📔🗂️", bgClass: "bg-lime-200", buttonClass: "bg-lime-500",shadowColor:"shadow-lime-500", buttonHover: "hover:bg-lime-600", buttonText: "بریم ببینیم!" },
  { path: '/salamat', name: "پنل سلامت🩺🥼", bgClass: "bg-sky-100", buttonClass: "bg-sky-500",shadowColor:"shadow-sky-500", buttonHover: "hover:bg-sky-600", buttonText: "بزن بریم!" },
  { path: '/note', name: "دفترچه یادداشت📒✏️", bgClass: "bg-yellow-200", buttonClass: "bg-yellow-500",shadowColor:"shadow-yellow-500", buttonHover: "hover:bg-yellow-600", buttonText: "ورود به دفترچه یادداشت" }
];
</script>

<template>
  <aside class="w-[350px] h-[180vh] shadow-lg p-4 rounded-lg">
    <h2 class="font-black text-3xl mb-6 text-center">پنل دسترسی سریع</h2>
    <section class="flex flex-col justify-center items-center gap-[35px] bg-white">
      <!-- استفاده از v-for برای تولید داینامیک منو -->
      <div 
        v-for="item in menuItems" 
        :key="item.path"
        :class="['w-[95%] h-[200px] flex flex-col justify-center items-center gap-[30px] rounded-lg shadow-xl animate__animated', 
                 // نمونه‌ای از انیمیشن‌ها (می‌توانید بر اساس نیاز تغییر دهید)
                 item.name === 'Exam' || item.name === 'Note' ? 'animate__slideInRight' : 'animate__slideInLeft', 
                 item.bgClass,item.shadowColor]"
      >
        <h3 class="text-2xl">{{ item.name }}</h3>
        <router-link :to="item.path">
          <button :class="['px-4 py-3 text-white rounded', item.buttonClass, item.buttonHover]">
            {{ item.buttonText }}
          </button>
        </router-link>
      </div>

      <!-- مورد لینک خارجی: ربات تلگرام -->
      <div class="w-[95%] h-[200px] bg-purple-200 flex flex-col justify-center items-center gap-[30px] shadow-purple-500 shadow-xl animate__animated animate__slideInLeft">
        <h3 class="text-2xl">ربات غربال 🤖</h3>
        <a target="_blank" href="https://t.me/student_math_bot">
          <button class="px-4 py-3 bg-purple-500 text-white hover:bg-purple-600 rounded">
            ورود به ربات تلگرام
          </button>
        </a>
      </div>
    </section>
  </aside>
</template>


  
  
  