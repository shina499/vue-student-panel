  
<script setup>
import Heading from "@/components/Header.vue"; // نام باید با حرف بزرگ باشد
import Footer from "@/components/Footer.vue"; // نام فایل و import یکسان باشد
import Sidebar from "./Sidebar.vue";
import Dashboard from "@/views/dashboard.vue";
import Exam from "@/views/exam.vue";
import Salamat from "@/views/salamat.vue";
import Note from "@/views/note.vue";

</script>

<template>
  <div class="flex flex-col height">
    <Heading /> <!-- اینجا هم باید با حرف بزرگ باشد -->
    <div class="flex p-2">
      <div>
        <Sidebar />
      </div>
      <div>
        <router-view />
      </div>
    </div>
    <Footer />
  </div>
</template>

<style>
.height{
  height: fit-content;
}
</style>