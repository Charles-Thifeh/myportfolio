<template>
  <div class="bg-gray-900">
    <div class="max-w-2xl mx-auto py-24 px-4 grid items-center grid-cols-1 gap-y-16 gap-x-8 sm:px-6 sm:py-32 lg:max-w-7xl lg:px-8 lg:grid-cols-2">
      <div>
        <h2 class="text-3xl font-extrabold tracking-tight text-white sm:text-4xl">Technical Specifications</h2>
        <p class="mt-4 text-gray-100">My skills</p>

        <dl class="mt-16 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 sm:gap-y-16 lg:gap-x-8">
          <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">HTML</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-green-500 h-1" style="width: 95%"></div>
                </div>
            </dd>
        </div>
        <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">CSS</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-blue-500 h-1" style="width: 82%"></div>
                </div>
            </dd>
          </div>
          <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">VUE</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-orange-500 h-1" style="width: 76%"></div>
                </div>
            </dd>
        </div>
        <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">LARAVEL</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-blue-500 h-1" style="width: 88%"></div>
                </div>
            </dd>
          </div>
          <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">PYTHON</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-green-500 h-1" style="width: 90%"></div>
                </div>
            </dd>
        </div>
        <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">JAVASCRIPT</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-orange-500 h-1" style="width: 78%"></div>
                </div>
            </dd>
          </div>
          <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">FIGMA</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-blue-500 h-1" style="width: 83%"></div>
                </div>
            </dd>
        </div>
        <div class="border-t border-gray-200 pt-4">
            <dt class="font-medium text-gray-100">FLUTTER</dt>
            <dd>
                <div class="w-full bg-gray-200 h-1 mb-6">
                <div class="bg-red-500 h-1" style="width: 55%"></div>
                </div>
            </dd>
          </div>
        </dl>
      </div>
      <div class="grid grid-cols-2 grid-rows-2 gap-4 sm:gap-6 lg:gap-16 lg:mt-48 comein">
        <img src="../assets/html5-brands.svg" class="w-16 h-16"/>
        <img src="../assets/css3-alt-brands.svg" class="w-16 h-16"/>
        <img src="../assets/vuejs-brands.svg" class="w-16 h-16"/>
        <img src="../assets/laravel-brands.svg" class="w-16 h-16"/>
        <img src="../assets/python-brands.svg" class="w-16 h-16"/>
        <img src="../assets/js-brands.svg" class="w-16 h-16"/>
        <img src="../assets/icons8-figma.svg" class="w-16 h-16"/>
        <img src="../assets/icons8-flutter.svg" class="w-16 h-16"/>
      </div> 
    </div>
  </div>
</template>

<script>
const features = [
  { name: 'Html', description: '' },
  { name: 'Css', description: '' },
  { name: 'Vue', description: '' },
  { name: 'Laravel', description: '' },
  { name: 'Python', description: '' },
  { name: 'JavaScript', description: '' },
  { name: 'Figma', description: '' },
  { name: 'Flutter', description: '' },
]

export default {
  setup() {
    return {
      features,
    }
  },
}
</script>