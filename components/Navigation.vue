<!-- https://www.youtube.com/watch?v=Q2gQ20Q-4Pk -->
<!-- https://www.youtube.com/watch?v=ehuMq4JiYgQ -->
<template>
    <nav class="bg-color shadow-lg ">
        <section class="container mx-auto ">
          <div class="sm:flex justify-between">
            <!-- Might have to change to NuxtLink -->
            <a href="/" class="text-color text-3xl font-bold p-3">Vexus</a>
            <ul class="text-color sm:self-center text-lg border-t sm:border-none">
              <li class="sm:inline-block">
                <!-- Will change hover effect later -->
                <a href="/" class="p-3 hover:bg-pink-500 px-3 py-1 rounded text-gray-700 hover:text-white font-semibold">Home</a>
              </li>
              <li class="sm:inline-block">
                <a href="/blog" class="p-3 hover:bg-pink-500 px-3 py-1 rounded text-gray-700 hover:text-white font-semibold">Blog</a>
              </li>
              <li class="sm:inline-block">
                <a href="/about" class="p-3 hover:bg-pink-500 px-3 py-1 rounded text-gray-700 hover:text-white font-semibold">About</a>
              </li>
              <li class="sm:inline-block">
                <a href="/contact" class="p-3 hover:bg-pink-500 px-3 py-1 rounded text-gray-700 hover:text-white font-semibold">Contact</a>
              </li>
            </ul>
          </div>
        </section>
    </nav>
</template>