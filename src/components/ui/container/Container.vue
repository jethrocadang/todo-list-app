<script setup lang="ts">
import type { HTMLAttributes } from 'vue'
import { cn } from '@/lib/utils'

const props = defineProps<{
    class?: HTMLAttributes['class']
}>()
</script>

<template>
    <div :class="cn( 
        'h-full mx-auto w-full max-w-screen-xl px-2.5 md:px-20 bg-green-200' ,props.class
        )">
        <slot />

    </div>
</template>