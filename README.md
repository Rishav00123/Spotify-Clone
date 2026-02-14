# Spotify Web Player Clone

A Spotify-inspired web music player built using HTML, CSS, and JavaScript.  
This project dynamically loads songs from a local folder and provides full playback controls with a responsive UI.

---

## Features

- Dynamic song loading from local folder
- Play / Pause functionality
- Next & Previous controls
- Volume control slider
- Interactive seekbar with real-time progress
- Play songs directly from trending cards
- Sidebar song list
- Responsive layout (mobile + desktop)
- Clean decoded song names (no %20 issue)

---

##  Tech Stack

- HTML5
- CSS3 (Flexbox + Media Queries)
- Vanilla JavaScript (ES6)
- JavaScript Audio API

---

##  Project Structure

project-folder/
│
├── index.html  
├── style.css  
├── utility.css  
├── script.js  
│  
├── spotify-songs/  
│   ├── song1.mp3  
│   ├── song2.mp3  
│   └── ...  
│  
├── spotify-img/  
│   ├── 1.jpg  
│   ├── 2.jpg  
│   └── ...  
│  
├── icons/  
│   ├── play.svg  
│   ├── pause.svg  
│   ├── next.svg  
│   ├── prev.svg  
│   └── volumeon.svg  

---

##  How It Works

### Song Fetching
The app fetches all `.mp3` files dynamically from the `spotify-songs` directory using `fetch()` and displays them in the sidebar.

### Audio Playback
A global `Audio()` object is used to control playback:
- play()
- pause()
- currentTime
- volume

### Seekbar Logic
The seekbar position is calculated using:

(currentTime / duration) * 100

Clicking on the seekbar updates the current playback position.

### Clean Song Names
Filenames are decoded using `decodeURIComponent()` to remove encoded characters like `%20`.

---

## 📱 Responsive Behavior

- Sidebar slides in/out on mobile using hamburger menu
- Cards resize automatically
- Playbar adapts for smaller screens
- Layout uses Flexbox for responsiveness

---

##  Key Concepts Practiced

- DOM manipulation
- Event handling
- Audio API usage
- URL decoding
- State management
- Responsive design
- Debugging z-index and stacking contexts

---

##  Future Improvements

- Shuffle mode
- Repeat mode
- Playlist creation
- Search functionality
- Backend integration
- Authentication system
- Database support

---

## ▶ How to Run

1. Clone the repository
2. Open the project folder
3. Run using Live Server (recommended)
4. Make sure your songs are inside the `spotify-songs` folder
5. Open in browser and enjoy 🎧

---

##  Disclaimer

This project is built for educational purposes only and is not affiliated with Spotify.
