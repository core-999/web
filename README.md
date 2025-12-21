# Website For Girlfriend

A fun, interactive web app that lets users choose their gift in a playful, cartoon-inspired style. Perfect for birthdays, celebrations, or simply adding some whimsy to any event!

## Overview

This repository contains a multi-page web application featuring a vibrant, cartoon-themed design. With engaging animations, interactive gift selections, and playful messaging, the app creates an unforgettable experience for users. Its versatile design makes it ideal not only for general gifting but also for birthday celebrations and special occasions.

## Features

### Cartoon-Inspired Design
- Uses playful Google Fonts ("Luckiest Guy" and "Comic Neue") along with vibrant gradients and animated elements.

### Interactive Gift Selection
- Multiple pages let users choose between different gift options, with fun hover effects, dynamic font sizing, and engaging alerts.

### Custom Gift Input
- A dedicated page where users can describe their custom gift wish.

### Playful Animations
- Bouncing headings, floating buttons, and animated images create a lively and engaging interface.

### Background Music
- Integrated looping background music enhances the overall interactive experience.

### Versatile Usage
- Designed for fun, the app can easily be adapted for birthday celebrations or any special event to make gifting interactive and memorable.

## Project Structure

```
cartoon-gift-selector/
├── index.html                 # Main page for gift selection
├── contact.html               # Page to describe a custom gift
├── question2.html             # Additional interactive page with playful questions
├── final.html                 # (Optional) Final page after selection
├── style.css                  # External stylesheet (if separated)
├── music/
│   └── ahatamatarmusic.mp3    # Background music file
└── img/
    ├── gift1.webp             # Image for Gift 1
    ├── gift2.png              # Image for Gift 2 & Custom Gift
    ├── sleep.webp             # Image used in question pages
    └── hamster.jpg            # Hamster image with animations
```

## Getting Started

To run this project locally:

1. Clone the repository:
    ```bash
    git clone https://github.com/pinakkk/Website-For-Girlfriend
    ```

2. Navigate to the project directory:
    ```bash
    cd website-for-girlfriend
    ```

3. Open the main HTML file in your web browser:
    - On macOS:
        ```bash
        open index.html
        ```
    - On Windows, simply double-click the file or right-click and select "Open with" your preferred browser.

4. Enjoy the interactive experience!

## Customization

Feel free to modify the content, styling, and animations to suit your needs. The project is built with standard HTML, CSS, and JavaScript, making it simple to extend and customize.

### For Birthday Celebrations

This web app is also perfect for birthday events! Update the text, images, and interactive messages to include birthday greetings and themed gift options. It’s an engaging way to surprise guests and create a memorable celebration experience.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Google Fonts

## License

This project is open source and available under the MIT License.

## Contributing

Contributions are welcome! Please feel free to fork the repository and submit pull requests with any enhancements or bug fixes. If you encounter any issues, open an issue on GitHub to discuss potential improvements.


## Deployment

### Deploy Frontend on Vercel

You can deploy this React frontend directly to Vercel using the button below:

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/Hkmusic/web>)

**Important:** Replace `<YOUR-GITHUB-USERNAME>` and `<YOUR-REPO-NAME>` with your actual GitHub username and repo name.

#### Fixing Peer Dependency Conflicts

Since `react-hls-player` has a peer dependency on React 16, Vercel build may fail. To fix it:

1. Add a **Vercel-specific build script** in `package.json`:

```json
"scripts": {
  "start": "craco start",
  "build": "craco build",
  "test": "craco test",
  "eject": "react-scripts eject",
  "vercel-build": "npm install --legacy-peer-deps && npm run build"
}

