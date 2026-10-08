# Bioengineering Week (Vue + Vite starter)

## Setup (once)
Install [Node.js](https://nodejs.org), then in this folder:

```
npm install
```

## Run it
```
npm run dev
```
Open the link it prints (usually http://localhost:5173). The page updates as you save files.

## Build for deployment
```
npm run build
```
The result goes in `dist/`.

## Where things are
- `src/App.vue`: the page, puts the components together (event name and date are set here)
- `src/components/`: one file per section (`HeroSection`, `ScheduleList`, `SignUpForm`)
- `src/data/activities.js`: the schedule
- `src/style.css`: global styles and colors (each component also has its own `<style scoped>`)

Each `.vue` file has three parts: `<script setup>` (logic), `<template>` (HTML) and `<style>` (CSS).

## Things to do
- Change the colors in `src/style.css`
- Add an activity in `src/data/activities.js`
- Add a new field to the sign-up form (for example, course or year)
- In the card elements of the schedule, add information about the location and date of each activity
- Stop people from signing up with the same email twice
- Create a new component, for example a `SpeakersSection.vue`
