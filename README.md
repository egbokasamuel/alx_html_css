# Headphones Web Page

This project is a fully functional web page created using HTML and CSS. It was developed to implement various web development skills, including HTML structure, CSS styling, responsive design, and accessibility practices.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Responsive Design](#responsive-design)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview
The Headphones web page was designed to showcase a fictional product line. It includes sections for the header, services, results, contact form, and footer. The design is responsive and adjusts for different screen sizes, ensuring a good user experience on both desktop and mobile devices.

## Features
- **Header Section**: Includes a hero image, title, description, and a call-to-action button.
- **What We Do Section**: Displays various services provided with icons and descriptions.
- **Results Section**: Highlights key results with statistics.
- **Contact Us Section**: Provides a form for users to get in touch.
- **Footer Section**: Contains company information and social media links.

## Technologies Used
- HTML
- CSS

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/alx_html_css.git
    ```
2. Navigate to the project directory:
    ```sh
    cd headphones
    ```

## Usage
1. Open `index.html` in your web browser to view the web page.

## Screenshots
![Headphones Web Page Screenshot](screenshot.png)

## Responsive Design
The webpage is fully responsive. It adjusts its layout based on the screen size:
- For screens 1000px wide or less, the layout changes to fit the screen better.
- For screens 480px wide or less, the layout switches to a mobile-friendly design.

### Media Queries Used:
```css
/* For screens 1000px wide or less */
@media (max-width: 1000px) {
    .services-container, .results-container {
        flex-direction: column;
        align-items: center;
    }

    .service, .result {
        width: 80%;
        margin-bottom: 20px;
    }
}

/* For screens 480px wide or less */
@media (max-width: 480px) {
    header .hero h1 {
        font-size: 1.8em;
    }

    header .hero p {
        font-size: 1em;
    }

    .services-container, .results-container {
        flex-direction: column;
        align-items: center;
    }

    .service, .result {
        width: 100%;
        margin-bottom: 20px;
    }

    .contact form input, .contact form textarea {
        width: 90%;
    }
}