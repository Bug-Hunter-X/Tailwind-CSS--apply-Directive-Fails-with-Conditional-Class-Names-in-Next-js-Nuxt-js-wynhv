# Tailwind CSS @apply Directive Bug in Next.js/Nuxt.js

This repository demonstrates a bug where the Tailwind CSS `@apply` directive fails to apply classes conditionally when dealing with dynamic class names in frameworks like Next.js or Nuxt.js. The issue is related to conditional rendering and the timing of the Tailwind compilation process.

## Problem

When using `@apply` with dynamic class names generated during runtime (e.g., within a loop or conditional statement), the compiler might not be able to resolve the class names at compile time, leading to missing styles. This makes it challenging to apply styles based on conditional logic.

## Solution

The solution involves restructuring your approach to avoid dynamically generating classes that need to be applied via `@apply`.  Instead, consider using direct class names or another method like styled-components, which provides more runtime flexibility.