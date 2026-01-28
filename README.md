🌹 Romantic Valentine Gesture Magic
An interactive, AI-powered web experience that uses Hand Gesture Recognition and 3D Particle Systems to create a magical Valentine's surprise.

📸 Preview
A swirling 3D heart made of 30,000 rose-petal particles reacts to your hand movements. Pinch your fingers to reveal a hidden romantic message.

✨ Features
🤖 AI Gesture Tracking: Real-time hand landmark detection using Google MediaPipe.

🌸 Rose Petal Particles: 30,000 high-performance 3D particles with additive blending for a glowing, romantic effect.

🎵 Integrated Music: Seamlessly loops a romantic soundtrack (activates on first interaction).

🖋️ Calligraphic Typography: Uses the Great Vibes font for an elegant, handwritten feel.

💖 Dynamic Scaling: The heart "pulses" and scales based on the distance between your thumb and index finger.

🛠️ Tech Stack
🚀 Quick Start
Clone this repository or download the index.html file.

Open index.html in a modern web browser (Chrome or Edge recommended).

Allow Camera Access when prompted.

Click anywhere on the screen to start the music.

The Magic Gesture: * Open your hand to grow the heart.

Pinch your thumb and index finger together to see the secret message.

🧠 How It Works
The project combines two powerful libraries:

MediaPipe Hands: Processes the webcam feed to locate 21 specific points on your hand. It calculates the distance between point 4 (Thumb Tip) and point 8 (Index Tip).

Three.js: Uses a parametric heart formula to plot thousands of points in 3D space.

JavaScript
// The heart is generated using this parametric formula:
const x = 16 * Math.pow(Math.sin(t), 3);
const y = 13 * Math.cos(t) - 5 * Math.cos(2*t) - 2 * Math.cos(3*t) - Math.cos(4*t);
📝 Customization
You can easily customize the experience in the script:

Change the Song: Replace the src in the <audio> tag.

Change Colors: Adjust the params.color hex code.

Adjust Density: Increase or decrease particleCount for different performance levels.

🔒 Privacy
No data is sent to a server.

All webcam processing happens locally in the browser using the client's GPU/CPU.

💌 Credits
Music: Bensound.com

Engine: Three.js & MediaPipe
