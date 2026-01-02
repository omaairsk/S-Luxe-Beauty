✨ S-Luxe Beauty | AI Virtual Skin Analysis & Shop
S-Luxe Beauty is a real-time web application that uses computer vision to analyze a user's skin tone via their webcam and automatically recommends beauty products tailored to their complexion. The app features a dynamic filtering system that sorts products from "Budget-Friendly" to "High-End Luxury."

Privacy First: All video processing happens 100% inside the user's browser. No images are ever sent to a server or stored.

🚀 Features
Real-Time Camera Access: Seamless integration with the device's webcam using the HTML5 MediaDevices API.

Client-Side "AI" Analysis: Algorithms analyze live video frames to calculate pixel luminance and determine skin tone (Fair, Medium, Dark).

Dynamic Product Recommendations: Automatically filters products based on the analysis results.

Price Tiering: Showcases products in two distinct categories: Cheap (Drugstore) vs. Expensive (Luxury).

Review System: Functional frontend for submitting and displaying user reviews.

Responsive UI: A modern, clean interface with modals for Login/Signup and a footer with social links.

🛠️ Tech Stack
Frontend: HTML5, CSS3 (CSS Variables, Flexbox/Grid).

Logic: Vanilla JavaScript (ES6+).

Computer Vision: HTML5 Canvas API & Pixel Manipulation.

No External Dependencies: Runs entirely without libraries like jQuery or React.

⚙️ How It Works (The Logic)
Stream Capture: The app requests permission to access the user's webcam (navigator.mediaDevices.getUserMedia).

Frame Sampling: When the user clicks "Analyze," the app captures the current video frame onto a hidden HTML Canvas.

Pixel Analysis:

The script extracts pixel data from the center of the frame (where the face/cheek is positioned).

It calculates the average RGB (Red, Green, Blue) values of that specific area.

Tone Calculation:

It converts the RGB values into Luminance (Brightness) using the formula: 0.2126*R + 0.7152*G + 0.0722*B.

Based on the brightness threshold, it categorizes the skin as Fair, Medium, or Dark.

DOM Manipulation: The JavaScript filters the JSON product list and injects the matching HTML cards into the view.

📦 How to Run Locally
Since this is a client-side application, you do not need to install Node.js or Python.

Clone the repository:

Bash

git clone https://github.com/omaairsk/s-luxe-beauty.git
Open the file: Navigate to the folder and double-click index.html (or sluxe_beauty.html) to open it in your default web browser (Chrome, Edge, or Firefox recommended).

Allow Permissions: When prompted by the browser, click "Allow" to grant camera access.

📸 Screenshots
(You can upload screenshots of your app here)

🔒 Privacy Policy
This application operates on a Zero-Data Retention policy:

Video feeds are processed in real-time within the browser's volatile memory.

No images are saved to a database.

No biometric data is transmitted over the internet.

🤝 Contributing
Contributions are welcome!

Fork the Project.

Create your Feature Branch.

Commit your Changes.

Push to the Branch.

Open a Pull Request.

📄 License
Distributed under the MIT License. See LICENSE for more information.

Created by [ OMAAIR SK ]
