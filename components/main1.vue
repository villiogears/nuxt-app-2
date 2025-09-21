<template>
  <div class="bg-white dark:bg-gray-900 text-gray-900 dark:text-white">
    <!-- Hero Section -->
    <section class="bg-gray-100 dark:bg-gray-800">
      <div class="container mx-auto px-4 py-20 text-center">
        <h1 class="text-4xl md:text-6xl font-bold tracking-tight">
          elphadeal
        </h1>
        <p class="mt-4 text-lg md:text-xl text-gray-600 dark:text-gray-300">
          portfolio
        </p>
        <div class="mt-8 flex justify-center gap-4">
          <NuxtButton size="xl" to="#about">
            About
          </NuxtButton>
        </div>
      </div>
    </section>

    <!-- About Section -->
    <section id="about" class="container mx-auto px-4 py-16">
      <div class="max-w-3xl mx-auto text-center">
        <h2 class="text-3xl font-bold">About Me</h2>
        <p class="mt-4 text-gray-600 dark:text-gray-300">
          I am elphadeal, I love Nuxt
        </p>
      </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="bg-gray-50 dark:bg-gray-800 py-16">
      <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-center mb-8">My Projects</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- Project Card 2 -->
        <div class="flex justify-center">
            <NuxtCard class="max-w-sm w-full center5 text-center">
                <template #header>
                    <h3 class="text-xl font-semibold">Project Title</h3>
                </template>
                <p class="text-gray-600 dark:text-gray-300">A brief description of the project goes here. Explain the purpose and the technologies used.</p>
                <template #footer>
                    <NuxtLink to="#" class="text-primary hover:underline inline-block mt-4">View Project &rarr;</NuxtLink>
                </template>
            </NuxtCard>
        </div>
        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="container mx-auto px-4 py-16">
        <h2 class="text-3xl font-bold text-center mb-8">My Skills</h2>
        <div class="max-w-4xl mx-auto">
            <div class="flex flex-wrap justify-center gap-4">
                <NuxtBadge size="lg" variant="solid">JavaScript</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">Vue.js</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">Nuxt.js</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">TypeScript</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">Tailwind CSS</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">Node.js</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">HTML5</NuxtBadge>
                <NuxtBadge size="lg" variant="solid">CSS3</NuxtBadge>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="bg-gray-50 dark:bg-gray-800 py-16">
      <div class="container mx-auto px-4">
        <div class="max-w-xl mx-auto">
        </div>
      </div>
    </section>
  </div>
</template>