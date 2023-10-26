# Nuxt devtools misleading css classes bug report

## Issue

The IDE WebStorm suggested `w-100` css class, but it actually cannot be used.

## Reproduce

1. Clone and open the project in WebStorm
2. Open app.vue
3. Put your cursor after `w-` in css class `w-100`
4. Hit `Ctrl + Space` to invoke suggestion
5. WebStorm suggest `w-100` as an option
6. Hit `Ctrl + B` to navigate to `w-100`'s declaration
7. It turns out to be `w-100` comes from an `entry.xxxxxxxx.css` file from `@nuxt/devtools`