<script setup>
const props = defineProps(['heading'])
</script>
<template>
    <header class="w-full h-[80px] bg-gray-100 ">
        <div class="flex justify-between items-center h-[80px] gap-[20px] p-5">

            <div class="flex flex-col gap-1">
                <p class="text-lg font-bold">خوش آمدید</p>
                <p class="text-sm font-light">امروز <span>یکشنبه ۱۲ اسفند</span></p>
            </div>
            
            <div class="flex gap-[10px] justify-center items-center">
                <!-- website icon -->
                <img class="w-[60px] h-[60px] rounded" src="../../public/favicon.png" alt="website-icon">
                <!-- website title -->
                <h1 class="text-2xl font-black">پنل دانش آموزی ایستگاه دانش</h1>
            </div>

            <div>
                <p class="text-lg font-bold">به نام خداوند جان و خرد</p>
            </div>
            
        </div>
    </header>
</template>
