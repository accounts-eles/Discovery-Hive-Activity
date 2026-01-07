🐝 Discovery Hive Activity
An interactive, "honeycomb" styled discovery activity built with Tailwind CSS and Vanilla JavaScript. This tool gamifies information retrieval by requiring users to explore a hexagonal grid to reveal hidden content, tracking their progress in real-time.

🚀 Live Demo
View the Live Activity Here

✨ Features
Gamified Exploration: Users interact with a "hive" of hexagons. Clicking "Content" nodes reveals information, while clicking "Filler" nodes causes them to vanish, clearing the board.

Dynamic Progress Tracking: A real-time progress bar calculates completion percentage based on the number of content items discovered per page.

Multi-Page Support: Includes a state-managed navigation system allowing for multiple "levels" or categories of discovery.

Modern UI/UX: * Glassmorphism: High-end modal backgrounds and blur effects.

Fluid Animations: Scale and color transitions using cubic-bezier timing.

Geometric Precision: Hexagons are rendered using CSS clip-path for a sharp, mathematical look without images.

Fully Responsive: Designed to scale beautifully across different screen sizes using Tailwind's utility-first framework.

🛠️ Technical Stack
HTML5: Structured for semantic accessibility.

Tailwind CSS: Used for rapid layout design and modern styling.

Vanilla JavaScript: Handles the game logic, state management (current page/revealed count), and DOM manipulation.

Google Fonts: Integrated 'Inter' font family for a clean, professional aesthetic.

📂 Project Structure
Plaintext

Discovery-Hive-Activity/
├── index.html          # Main application file (UI + Logic)
├── previews/           # Auto-generated social preview thumbnails
└── .github/workflows/  # Automation for thumbnail generation
⚙️ Configuration
The content of the hive is easily customizable via the pages constant in the <script> section. You can add as many pages or hexagons as needed:

JavaScript

const pages = [
    {
        title: "Your Custom Title",
        desc: "Instructions for the user...",
        hexagons: [
            { type: 'content', heading: "Visible Title", text: "Hidden information..." },
            { type: 'filler', text: "Optional label" }
        ]
    }
];
🤖 Automation
This repository is integrated with a GitHub Actions workflow that:

Monitors changes to the code.

Launches a headless browser (Puppeteer).

Captures a high-resolution screenshot of the live activity.

Commits the thumbnail to the previews/ folder for use in the Catalog of Repos.

📄 License
MIT License - Feel free to use and modify for your own interactive projects.
