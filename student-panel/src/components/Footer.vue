<script setup>
const props = defineProps(['Footer'])
</script>
<template>
    <footer class="w-full  bg-gray-200 flex justify-between items-center p-15">

<div class="flex flex-col justify-center">
    <h3 class="text-xl text-gray-800 font-black">با ما در ارتباط باشید</h3>
    <ul class="flex flex-col justify-center">
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://web.shad.ir/">شاد</a></li>
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://web.rubika.ir/">روبیکا</a></li>
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://web.splus.ir/">سروش پلاس</a></li>
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://bale.ai/">بله</a></li>
    </ul>
</div>

<div class="flex flex-col justify-center">
    <h3 class="text-xl text-gray-800 font-black">در پروژه ما همکاری کنید</h3>
    <ul class="flex flex-col justify-center">
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://github.com/shina499">گیت هاب</a></li>
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://www.instagram.com/">اینستاگرام</a></li>
        <li class="text-gray-400 text-lg hover:text-gray-500"><a href="https://www.linkedin.com/in/n-hosseiny-hosseiny-781256349/">لینکدین</a></li>
    </ul>
</div>

<div class="flex flex-col gap-2">
    <figure>
        <a href="#">
            <img src="../../public/favicon.png" class="w-[120px] h-[120px] rounded" alt="icon">
        </a>
    </figure>
    
    <span class="text-center text-gray-700 text-lg">ایستگاه دانش</span>
</div>

<p class="text-xl">ساخته شده با ❤️ در گروه برنامه سازان آینده</p>
</footer>
</template>