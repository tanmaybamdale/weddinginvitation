Shubh Vivah - Cinematic Wedding Invitation Website

A luxurious, interactive wedding invitation designed to play like a video. This project uses pure HTML, CSS (Tailwind), and Vanilla JavaScript to create a storytelling experience that guides the guest through the wedding details sequentially.

✨ Features

Cinematic Loader: A custom 8-second animated intro screen (#video-loader) to build anticipation.

"Video" Timeline Logic: The page automatically scrolls and reveals sections (Intro -> Date -> Couple -> RSVP) using a JavaScript sequencing engine, mimicking a video presentation.

Atmospheric Effects: A high-performance HTML5 Canvas background rendering falling rose petals and gold ribbons.

Royal Indian Aesthetic: Designed with a Pune/Marathi wedding context in mind, using a Maroon, Gold, and Cream color palette.

Single File Architecture: All CSS, JS, and HTML are contained in one file for easy sharing and hosting.

Responsive: Fully adaptive layout using Tailwind CSS.

🛠️ Tech Stack

HTML5

Tailwind CSS (via CDN)

Vanilla JavaScript (No heavy frameworks like React/Vue required)

Google Fonts (Great Vibes, Cinzel, Lato)

🚀 How to Run

Clone the repository:

git clone [https://github.com/yourusername/wedding-invite.git](https://github.com/yourusername/wedding-invite.git)


Open the file:
Simply double-click wedding_invite.html to open it in any modern browser (Chrome, Firefox, Safari). No server is required!

⚙️ Customization Guide

To personalize this invitation for your own wedding, open wedding_invite.html in a text editor (like VS Code or Notepad) and edit the following sections:

1. Changing Names & Text

Look for the text content within the HTML tags.

Bride & Groom: Search for "Aarav Patil" or "Ananya Deshmukh".

Dates: Search for "Dec 14, 2025".

Venue: Search for "Grand Hyatt Pune".

2. Changing Images

Replace the placeholder URLs in the <img> tags with your own hosted image links:

<img src="YOUR_IMAGE_URL_HERE" alt="Groom" class="couple-img">


3. Adding Music

To make the Music Button functional, add an audio tag inside the <body> and update the JavaScript:

Add HTML:

<audio id="bg-music" loop>
    <source src="./music/wedding-shenai.mp3" type="audio/mpeg">
</audio>


Update JS (toggleMusic function):

const audio = document.getElementById('bg-music');
// Inside the if(!musicPlaying) block:
audio.play();
// Inside the else block:
audio.pause();


4. Adjusting Timing

You can speed up or slow down the "video" flow by changing these constants in the <script> section:

const LOADER_DURATION = 8000; // 8 seconds for intro
const SCENE_DURATION = 5000;  // 5 seconds per slide


📄 License

This project is open source and available for personal use.

Made with ❤️ for the happy couple.
