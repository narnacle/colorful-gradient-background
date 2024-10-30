# Colorful Gradient Background Animation

This project demonstrates a **colorful, animated gradient background** using pure HTML and CSS. The background smoothly transitions between various colors, creating an eye-catching effect suitable for web projects, landing pages, or background elements.

## Demo

![Animated Gradient Background](demo.gif)

## Features

- **Smooth Color Transitions**: The background smoothly cycles through a series of colors.
- **Customizable Gradient**: Easily change colors, animation speed, and direction.
- **Pure CSS Implementation**: No JavaScript or external libraries are needed.

## Getting Started

To use this animated background, simply copy the HTML and CSS code provided below and include it in your project.

### Prerequisites

This project requires only basic HTML and CSS knowledge. No additional tools or libraries are needed.

## Usage

1. **Copy the Code**: Copy the code below into your project.

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Animated Gradient Background</title>
      <style>
        /* Make the entire page fill the viewport */
        body, html {
          height: 100%;
          margin: 0;
          overflow: hidden;
        }

        /* The gradient animation */
        .gradient-background {
          width: 100%;
          height: 100%;
          background: linear-gradient(45deg, #ff9a9e, #fad0c4, #fbc2eb, #a18cd1, #fbc2eb);
          background-size: 300% 300%;
          animation: gradientAnimation 10s ease infinite;
        }

        /* Keyframes for the gradient animation */
        @keyframes gradientAnimation {
          0% { background-position: 0% 50%; }
          50% { background-position: 100% 50%; }
          100% { background-position: 0% 50%; }
        }
      </style>
    </head>
    <body>
      <div class="gradient-background"></div>
    </body>
    </html>
    ```

2. **Adjust as Needed**:
    - Modify the gradient colors, speed, or direction by changing the CSS in the `.gradient-background` class.
    - Customize the animation speed by adjusting the `10s` in the `animation` property.

## Customization

- **Change Colors**: Update the colors in the `linear-gradient` function.
- **Adjust Animation Speed**: Modify the `10s` in `animation: gradientAnimation 10s ease infinite;` to control the transition speed.
- **Change Direction**: Adjust the angle in `linear-gradient(45deg, ...);` to alter the gradient direction.

## Example Applications

- Landing pages and splash screens
- Web application backgrounds
- Loading screens or fullscreen backgrounds

## Contributing

If you’d like to contribute, please fork the repository and submit a pull request. We welcome any improvements, bug fixes, or suggestions!

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.
