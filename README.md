Year With You 4534
Overview

Year With You is a cinematic, scroll-driven digital storytelling experience designed as an interactive love letter. It presents memories and emotions through smooth transitions, synchronized audio, images, and video that unfold progressively as users scroll.

Built using modern frontend technologies, the project focuses on immersive storytelling, fluid motion design, and structured pacing. The application runs entirely on the client side with locally stored media assets and requires no backend services, database, or authentication.

Tech Stack

Next.js (App Router) – Routing and application structure

Tailwind CSS – Styling and responsive layout

Framer Motion – Animations and motion effects

Local Media Assets – Audio, images, and videos stored in /public

Features

Scroll-driven cinematic storytelling

Smooth animated transitions between chapters

Audio playback with seamless crossfading

Memory sections with images and videos

IntersectionObserver-based active section detection

Long-press interaction to reveal a hidden message

Fully client-side implementation

Getting Started
Installation
npm install
npm run dev

Open your browser and visit:

http://localhost:3000
Media Assets

Place your media files inside the /public directory using the following structure:

/public/audio/heartbeat.mp3
/public/audio/*.mp3
/public/images/*.jpg
/public/images/*.png
/public/video/*.mp4
/public/images/song-*.jpg

Story content and asset references are defined in:

data/story.ts
Project Structure
app/page.tsx
components/year-with-you-experience.tsx
hooks/use-dual-audio.ts
hooks/use-intersection-active.ts
data/story.ts
app/globals.css
Interaction Notes

Audio begins only after the user clicks Start Our Story due to browser autoplay policies.

Music transitions between memory sections crossfade over approximately 3.5 seconds.

The final scene fades music out gradually over 8 seconds.

A 3-second long press interaction reveals a hidden message.

Purpose

This project demonstrates how modern frontend tools can be used to create immersive narrative-driven web experiences. It highlights animation workflows, media synchronization, and interactive storytelling within a purely client-side environment....
