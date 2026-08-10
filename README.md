DesignT - A Modern, Customizable New Tab Page

DesignT is a feature-rich, high-performance browser New Tab page built entirely with vanilla HTML, CSS, and JavaScript. It operates without frameworks, build steps, or external dependencies. The application is engineered to provide a clean, highly personalized dashboard experience with extensive customization capabilities.

Features
Dynamic Search and Taskbar

     Multi-Engine Search: Choose between DuckDuckGo, Google, GitHub, YouTube, Wikipedia, or add custom search engines.
     Customizable Search Bar: Independently configure the search bar's background, text color, border color, and placeholder text.
     XYZ Dimensions: Control the Width (X), Height/Thickness (Y), and Elevation/Shadow depth (Z) of the search bar.
     Center Taskbar Button: An optional, customizable call-to-action button (e.g., "Launch Dashboard").

Glassmorphism Shortcuts

     Automatic High-Resolution Icons: Automatically fetches high-resolution favicons for shortcuts. Custom image URLs are also supported.
     Placeholder Tiles: Empty grid spaces are populated with functional placeholder tiles that immediately open the settings menu upon interaction.
     Fully Scalable: Adjust tile box size, icon size, label font size, and label position (Top, Bottom, or Hidden).
     Quick Edit Menu: Hovering over a shortcut reveals a quick edit and delete dropdown.

Weather Widget

     Real-Time Data: Powered by the free and reliable Open-Meteo API.
     City Autocomplete: Typing a city name triggers a dropdown of exact matches. Alternatively, the field can be left empty to utilize browser GPS.
     High-Quality Icons: Utilizes the basmilius/weather-icons repository for high-resolution animated SVG icons.
     Dynamic Theming: The widget strictly adapts to the current color palette and border radius settings.

Widgets and Integrations

     Custom Code Widget: Supports custom HTML, CSS, and JavaScript input directly within the settings, rendering output in the top-left corner.
     Mini GitHub Widget: A compact, integrated link to a specified GitHub profile adjacent to the settings button.

Advanced Theming and Design Language

     Preset Themes: Includes Gruvbox (default), Original Dark, Nord, Dracula, and Monochrome.
     Custom Colors and Gradients: Supports custom background and foreground colors, alongside linear, radial, and conic gradients with three color stops and adjustable angles.
     Custom Backgrounds: Users can upload an image from their device to use as a full-screen background.
     Unified Radius Scaling: A single border radius slider controls the sharpness of all UI elements, including the search bar, shortcut boxes, and the weather widget.
     Typography: Choose between Open Sans (Qwant's official font), Inter, Roboto, System UI, or Fira Code.

Decluttered Settings UI

     Searchable Settings: A built-in search bar instantly filters and highlights relevant configuration sections.
     Collapsible Accordions: Settings are grouped into logical, collapsible sections to maintain a clean and navigable interface.
     Instant Saving: Adjustments apply and save instantly, eliminating the need to save after every minor change.
     Import/Export: Back up the entire configuration (shortcuts, colors, dimensions, etc.) as a JSON string. Includes a Shadcn-style copy-to-clipboard button.

Tech Stack and Design Language

DesignT is built on modern web standards without relying on heavy frameworks. 

     Vanilla JavaScript: Pure JS implementation for optimal performance and negligible load times.
     CSS Variables (:root): The UI is driven by CSS custom properties. Changing a single variable instantly themes the entire page.
     color-mix() in CSS: Used to create dynamic, semi-transparent backgrounds and borders that adapt to the chosen color palette.
     backdrop-filter: blur(): The core of the glassmorphism design language, providing the frosted glass effect on the search bar, shortcuts, and widgets.
     Open-Meteo and Geocoding APIs: Used for weather data and city autocomplete without requiring API keys.

Installation and Usage

Because DesignT is a single HTML file, deployment is straightforward.
Option 1: Local Browser Homepage

    Download the index.html file.
    In your browser settings, set your homepage or new tab page to the local file path of the downloaded HTML file. Extensions like New Tab Override for Firefox or Custom New Tab URL for Chrome facilitate this process.

Option 2: Self-Hosting

    Upload the index.html file to any static web host (GitHub Pages, Netlify, Vercel, Cloudflare Pages).
    Point your browser's new tab page to the hosted URL.

Option 3: Browser Extension

DesignT can be wrapped into a Chrome or Firefox extension:

    Create a folder containing the index.html file.
    Add a manifest.json file to the directory:
    json
     
      
     
     
    {
      "name": "DesignT New Tab",
      "version": "1.0",
      "manifest_version": 3,
      "chrome_url_overrides": {
        "newtab": "index.html"
      }
    }
     
     
    Load the folder as an unpacked extension in your browser's developer settings.

Credits and Acknowledgments

     Author: Kamaldins
     Weather Data: Open-Meteo
     Weather Icons: basmilius/weather-icons
     Font Provider: Google Fonts (Open Sans, Inter, Roboto, Fira Code)
     Favicons: DuckDuckGo Icon Service

License

This project is open source. Feel free to fork, modify, and distribute it. If you find this project useful, a star on the repository is appreciated.
