<template>
  <div class="py-12 bg-gray-900" id="contacts">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="lg:text-left">
        <h2 class="text-3xl font-extrabold tracking-tight text-white sm:text-4xl">Contact Me</h2>
        <p class="mt-2 text-gray-400">
          Akinmusire Charles Boluwatife [Charles Thifeh]
        </p>
        
      </div>

      <div class="mt-10">
        <dl class="space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">
          <div v-for="feature in features" :key="feature.name" class="relative">
            <a :href="feature.href">
              <dt>
              <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                <component :is="feature.icon" class="h-6 w-6" aria-hidden="true" />
              </div>
              <p class="ml-16 text-lg leading-6 font-medium text-white">{{ feature.name }}</p>
            </dt>
            <dd class="mt-2 ml-16 text-base text-gray-500">
              {{ feature.description }}
            </dd>
            </a>
          </div>
        </dl>
      </div>
    </div>
  </div>
</template>

<script>
import { PhoneIcon, CodeIcon, InboxIcon, MailIcon } from '@heroicons/vue/outline'

const features = [
  {
    name: 'GitHub',
    description:
      'Charles-Thifeh',
    icon: CodeIcon,
    href: "https://github.com/Charles-Thifeh"
  },
]

export default {
  setup() {
    return {
      features,
    }
  },
}
</script>
