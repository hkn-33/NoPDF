<script setup>
  const props = defineProps({
    to: {
      type: String,
      default: null,
    },
    variant: {
      type: String,
      default: 'primary',
    },
  })

  const variants = {
    primary: 'bg-blue-600 text-white hover:bg-blue-700 shadow-blue-100 px-5 ',
    github:
      'bg-slate-900 text-white hover:bg-slate-800 shadow-slate-200 p-2.5 ',
    coffee:
      'bg-[#FFDD00] text-slate-900 hover:bg-[#FFCC00] shadow-yellow-100 px-5 ',
  }

  const baseCLasses =
    'flex items-center justify-center gap-2 rounded-full py-2.5 font-bold shadow-lg active:scale-95 transition-all'

  const buttonClass = computed(() => {
    return `${baseCLasses} ${variants[props.variant]}`
  })
</script>

<template>
  <NuxtLink :to="to" :class="buttonClass">
    <slot />
  </NuxtLink>
</template>
