# Album Tracker

A React web application that helps users discover and organize their music listening experience by searching albums and artists, previewing tracks, maintaining a personal listening collection with statuses, ratings, and notes, playing full albums through Deezer, and receiving AI-powered album recommendations based on their listening preferences.


**Live site:** https://album-tracker-rose.vercel.app

## Features
- Search albums and artists with the iTunes Search API
- Album page with cover, year, genre, track list, and 30-second previews
- Mini player that keeps playing while you browse
- Personal collection with status, 1-5 star rating, notes, filters, and sorting
- Optional full-album playback through the Deezer player
- LLM-powered recommendations based on your saved albums and ratings

## Tech stack
React, Vite, Context API, iTunes API, Deezer, Google Gemini, Vercel

## Run locally
1. `git clone "https://github.com/marcjustinebelen-cvsu/album-tracker.git"
2. `cd album-tracker`
3. `npm install`
4. Create `.env.local` with `GEMINI_API_KEY=your-key-here`
5. `npm run dev`

## Limitations
- Previews are 30 seconds (the most the iTunes API provides)
- The collection is saved only in your browser
- Deezer requires a login (and a plan in your country) for full tracks

## Privacy
The recommendations feature sends your saved albums' titles, artists, ratings, and statuses to Google's Gemini API. Your notes are not sent.

## Disclaimer
This is a learning project and is not affiliated with Apple, Spotify, Deezer, or Google. Music data, artwork, and audio belong to their owners.