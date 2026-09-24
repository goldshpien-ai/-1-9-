# 📱 Image Tracking with AR.js & MindAR

This project is a **minimal example** of using **[AR.js](https://ar-js-org.github.io/AR.js/)** with **[MindAR](https://hiukim.github.io/mind-ar-js-doc/)** for **image tracking** in the browser.
It detects a target image through the camera and overlays an image, GIF, or video on it.

---

## 🚀 Demo
Open the project in a mobile browser that supports WebXR (e.g., Chrome for Android) and point the camera at the target image.

---

## Project Structure
```
├── assets
│ ├── images/ # Overlay and target assets
│ │ ├── overlay.png # Example static overlay
│ │ ├── overlay.mp4 # Example video overlay
│ │ └── targets.mind # MindAR compiled target file
│ └── targets/ # Source marker images for MindAR
├── index.html # Main AR page
└── README.md # Project documentation
```

---

## 🛠 Requirements
- A modern browser with **WebXR / WebAR support**
- HTTPS hosting (AR requires secure context)
- Target `.mind` file generated with [MindAR CLI](https://hiukim.github.io/mind-ar-js-doc/tools/compile/)

---

## 📥 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/ehabAbdelMawla/mindar-image-tracking
   cd mindar-image-tracking

Serve App with https

https://localhost:5173

Point your camera to the target (marker) image.


🎥 Overlay Options
- Static Image
```
<a-plane src="#card" position="0 0 0" height="0.552" width="1"></a-plane>

```
- Video

Add <video> in <a-assets>
```

<video id="card" src="assets/images/overlay.mp4" autoplay loop muted></video>
```


On user interaction (required by most browsers):

```
window.addEventListener("click", () => {
  const vid = document.querySelector("#card");
  vid.play().catch(e => console.log("Video play error:", e));
});
```


 ## Connect With Me

<p align="center">
<a  href="mailto:eabdo1474@gmail.com">
 <img src="https://user-images.githubusercontent.com/51888513/188922645-da22d955-0b02-46d9-8145-564b54316d87.png" width="50"/> 
</a>
<a href="https://www.youtube.com/channel/UCnoe7bD7w2fWYlNzqY3qjLA">
<img src="https://user-images.githubusercontent.com/51888513/188924271-4554ab67-60b6-46db-9d38-b5d284bfc324.png" width="50"/>
</a>
<a href="https://www.linkedin.com/in/ehab-abdel-mawla-9b20aa183">
<img src="https://user-images.githubusercontent.com/51888513/188924356-4578aa1f-26c0-4310-a16d-f4eb3c891b8d.png" width="50"/>
</a>
<a href="https://codepen.io/ehabAbdelMola"><img src="https://user-images.githubusercontent.com/51888513/188924374-5169b372-1eda-4639-95b7-ceacbe31b861.png"   width="50"/> </a>
<a href="https://www.instagram.com/abdoehab4551/"><img src="https://user-images.githubusercontent.com/51888513/188924858-1b4bd316-4259-4f22-be15-0872c31ebc12.png"   width="50"/> </a>

</p>

