<template>
  <div class="bg-gray-800" id="projects">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="max-w-2xl mx-auto py-16 sm:py-24 lg:py-32 lg:max-w-none">
        <h2 class="text-3xl font-extrabold tracking-tight text-white sm:text-4xl">Projects</h2>

        <div class="mt-6 space-y-12 lg:space-y-0 lg:grid lg:grid-cols-3 lg:gap-x-6">
          <div v-for="callout in callouts" :key="callout.name" class="group relative">
            <div class="relative w-full h-80 bg-white rounded-lg overflow-hidden group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1 mt-8">
              <img :src="callout.imageSrc" :alt="callout.imageAlt" class="w-full h-full object-center object-cover" />
            </div>
            <h3 class="mt-6 font-bold text-sm text-gray-100">
              <a :href="callout.href">
                <span class="absolute inset-0" />
                {{ callout.name }}
              </a>
            </h3>
            <p class="text-base text-sm text-gray-400">{{ callout.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const callouts = [
  {
    name: 'School e-Portal',
    description: 'Created for oakfield schools. An e-portal for educational purpose. HTML, CSS, JS, Bootstrap, LARAVEL.',
    imageSrc: 'http://localhost/src/assets/sportal.PNG',
    imageAlt: 'oakfieldschools portal',
    href: 'https://oakfieldschools.com',
  },
  {
    name: 'DDoS Detect',
    description: "An implemented svm algorithm of a distributed denial of service attack using python. I ran this on a local server though. I can't afford the real one. HTML, CSS, JS, Bootstrap, Python Flask.",
    imageSrc: 'http://localhost/src/assets/ddosdetect.PNG',
    imageAlt: 'ddosdetect github',
    href: 'https://github.com/Charles-Thifeh/smartDDoSDetector',
  },
  {
    name: 'School Website',
    description: 'Created for oakfield schools. A website for the school. HTML, CSS, JS, LARAVEL.',
    imageSrc: 'http://localhost/src/assets/sweb.PNG',
    imageAlt: 'oakfieldschools website',
    href: 'https://site.oakfieldschools.com',
  },
  {
    name: 'My Portfolio',
    description: 'Where you at right now. HTML, CSS, JS, VUE js, Tailwind CSS.',
    imageSrc: 'http://localhost/src/assets/mp.PNG',
    imageAlt: 'My Portfolio',
    href: 'https://charlesthifeh.netlify.com',
  },
]

export default {
  setup() {
    return {
      callouts,
    }
  },
}
</script>
