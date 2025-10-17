# CAPTCHA Handler UI

A simple, client-side web application designed to display CAPTCHA images and allow users to input the perceived text. This utility is built with HTML and styled using Tailwind CSS, providing a responsive interface for handling various CAPTCHA images, including a default sample.

## Features

*   **Dynamic Image Loading**: Displays CAPTCHA images from a URL specified in the query string (`?url=https://.../image.png`) or from an input field.
*   **Default Sample Image**: If no URL is provided, it defaults to `sample.png`.
*   **User Input**: Provides a dedicated input field for users to enter the CAPTCHA text.
*   **Client-side "Verification"**: For the `sample.png`, it includes a basic client-side check against a known value ("ADJ R3"). For external images, it simply echoes the user's input, as real CAPTCHA verification requires a server-side component.
*   **Responsive Design**: Utilizes Tailwind CSS for a mobile-first, responsive user experience.

## Getting Started

To run this application, simply open the `index.html` file in your web browser. Ensure that `sample.png` is located in the same directory as `index.html`.

### Usage

1.  **Open `index.html`**: Navigate to the `index.html` file in your browser.
2.  **Load Custom CAPTCHA (Optional)**:
    *   You can append a `?url=` parameter to the browser's address bar (e.g., `index.html?url=https://example.com/captcha.png`).
    *   Alternatively, paste an image URL into the "Image URL" field and click "Load Image".
3.  **Enter CAPTCHA Text**: Type the text you see in the displayed image into the "Enter CAPTCHA text" field.
4.  **Verify**: Click "Verify CAPTCHA" to see the result. For `sample.png`, it will indicate if your input matches. For other images, it will show what you entered.

## Technologies Used

*   **HTML5**: Structure of the web page.
*   **Tailwind CSS**: Utility-first CSS framework for styling and responsiveness.
*   **JavaScript**: For dynamic image loading, user interaction, and client-side logic.

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.