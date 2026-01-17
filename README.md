# Riffly Music Player

Riffly is a sleek, fully functional web-based music player. It allows users to manage a dynamic playlist, control playback with precision, and experience a customized listening session through shuffle and delete functionalities.

---

![img](https://github.com/Faraz-Ali-1/Riffly-Music-Player/blob/8ae19ea00c6514df03b75646e8be94f71fea41e9/screenshots/riffly%201.jpg)

---

## Live Demo

https://faraz-ali-1.github.io/Riffly-Music-Player/

---

## Technical Features

### Comprehensive Playback Control
Implemented core audio features including Play, Pause, Next, and Previous. The player tracks the `currentTime` of the `Audio` object, ensuring that if a song is paused and resumed, it picks up exactly where it left off.

### Advanced Array Logic (Shuffle & Sort)
Developed a shuffle algorithm using `Math.random()` to reorder the playlist. The app also features an initial sorting logic that organizes the library alphabetically by song title upon loading or resetting.

### Dynamic Playlist Management
Users can remove songs from their current session. The logic handles edge cases—such as stopping the player if the currently playing song is deleted—and offers a "Reset Playlist" option once the library is empty.

### Data-Driven UI Rendering
Utilized a central `userData` object to keep the UI in sync with the state. The playlist is rendered dynamically using the `.map()` method, and the "Currently Playing" highlight is managed through real-time attribute updates.

---

## Technical Challenges

### Handling Audio State & Transitions
A major challenge was managing the transition when a song ends. I implemented an event listener for the `ended` state that automatically checks if a next song exists in the array and triggers the playback, creating a seamless automated listening experience.

### Maintaining Accessibility
I prioritized accessibility by implementing dynamic `aria-label` updates. Whenever the song changes, the "Play" button's accessible text updates to reflect the specific song title, ensuring the app is usable for people using screen readers.

---

![img](https://github.com/Faraz-Ali-1/Riffly-Music-Player/blob/8ae19ea00c6514df03b75646e8be94f71fea41e9/screenshots/riffly%202.jpg)

---

## Tech Stack

* **Logic:** Vanilla JavaScript (ES6+)
* **Media:** HTML5 Audio API
* **State Management:** Local Object-based state (userData)
* **Styling:** CSS3 (Modern Audio Player UI)

---

## Installation

1. Clone the repository.
2. Open `index.html` in your browser.
3. Use the control bar at the bottom to play, shuffle, or skip tracks.

---

## License

This project is licensed under the MIT License.
