# Petpet Gif Generator - Online Petting Animation GIF Maker

## Project Introduction

Petpet Gif Generator is a free online tool that allows users to create popular "pet-pet" animated GIFs, also known as petting GIFs and head pat GIFs, from any image. These animations show a hand affectionately patting the subject of your image, creating a cute and wholesome effect that's perfect for social media, messaging apps, and forum reactions.

## Features

### 🐾 Animation Types
- **Petting GIFs**: Feature a gentle hand motion that caresses the subject of your image, creating a warm and loving effect
- **Head Pat GIFs**: Showcase a playful hand motion that pats the top of your subject's head, conveying approval, encouragement, or simple affection

### ✨ Core Features
- **Easy Upload**: Support uploading any image from local files or URLs
- **Real-time Preview**: Instantly view animation effects and adjust parameters in real-time
- **Custom Controls**:
  - Adjust image size and position
  - Control animation speed (FPS)
  - Set squish effect intensity
  - Flip image orientation
  - Precise adjustment mode
- **High-quality Export**: Generate smooth, professional GIF animations
- **Responsive Design**: Perfectly adapts to desktop and mobile devices

### 🔧 Technical Features
- **Client-side Processing**: All image and GIF generation happens in the browser, ensuring privacy and speed
- **High-performance Rendering**: Optimized image processing and animation rendering using Canvas API
- **Advanced GIF Engine**: Built on gif.js, supporting high-quality GIF generation
- **Real-time Preview System**: Immediate feedback for all adjustments

## How to Use

### 1. Choose an Image
- Click the upload area or drag and drop files to upload any image from your device
- Supports all common image formats (PNG, JPG, JPEG, GIF, etc.)
- Square images work best, but any image will be automatically adjusted

### 2. Customize Animation
- Use the control interface to adjust:
  - **Size**: Adjust the scaling ratio of the main image
  - **Squish**: Control the intensity of the squish effect in the animation
  - **Speed**: Adjust the animation playback speed (2-60 FPS)
  - **Flip**: Horizontally flip the main image
  - **Adjust Mode**: Precisely adjust the position of the main image

### 3. Control Playback
- Play/pause the animation
- View animation effects frame by frame
- Reset all settings to default values

### 4. Export GIF
- Click the "Export" button to generate the GIF animation
- Wait for generation to complete (progress is displayed in real-time)
- Download the generated GIF file and share

## Technology Stack

- **Frontend Framework**: Vanilla JavaScript (ES6+)
- **Image Processing**: Canvas API
- **GIF Generation**: gif.js
- **Styling**: sanitize.css, Custom CSS Grid Layout
- **Icons**: jam-icons
- **Fonts**: Balsamiq Sans, Work Sans (Google Fonts)

## Project Structure

```
├── assets/
│   ├── gif.js              # GIF generation library
│   ├── main.js             # Main application logic
│   ├── requestInterval.js  # Animation interval control
│   └── style.css           # Main stylesheet
├── img/
│   ├── favicon-*.png       # Website icons
│   ├── manifest.json       # Web application manifest
│   ├── sample.png          # Default sample image
│   ├── sprite.png          # Hand gesture sprite
│   └── template.gif        # Animation template
├── gif.worker.js           # GIF generation worker thread
├── index.html              # Main page
├── README.md               # Project documentation (Chinese)
└── README_EN.md            # Project documentation (English)
```

## Core Algorithms

### Animation System
- 5-frame loop animation, simulating real petting/patting actions
- Each frame contains precise position, size, and deformation parameters
- Supports custom frame rate and delay settings

### Image Processing
- Automatic image scaling and caching for improved performance
- Support for cross-domain image loading
- Transparency handling optimization (using green background as transparent channel)

### GIF Generation
- Parallel processing of multiple frames using Web Workers
- Optimized color processing and transparency conversion
- Real-time progress feedback

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Privacy Policy

All image processing happens directly in your browser and is not uploaded to any server. Generated GIFs only exist in your browser's memory until you download them.

## License

This project is licensed under the MIT License.

## Contribution

Issue reports and Pull Requests are welcome!

## Contact

For questions or suggestions, please contact:
- Project URL: [https://github.com/dongyubin/petpet-gif-generator](https://github.com/dongyubin/petpet-gif-generator)

---

Create cute petting GIFs and head pat GIFs with Petpet Gif Generator, adding vitality and fun to your images! 🎉