<script setup>
import image from "@/assets/Capture.png";
</script>

<template>
    <nav class="bg-gray-600 w-full h-20 flex">
        <img :src="image" alt="img" class="w-20 h-20 ml-10"/>
        <div className="flex items-center">
            <ul className="flex flex-row text-white text-lg">
          <li>
            <a
              href="#"
              className="mx-10"
              >Menu 1</a
            >
          </li>

          <li>
            <a
              href="#"
              className="mx-8"
              >Menu 2</a
            >
          </li>

          <li>
            <a
              href="#"
              className="mx-8"
              >Menu 3</a
            >
          </li>
        </ul>
        </div>
    </nav>
</template>