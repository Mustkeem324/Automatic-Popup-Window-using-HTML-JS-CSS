# Automatic Popup Window using HTML, JS, CSS

## Overview

This project demonstrates how to create an automatic popup window using HTML, JS, and CSS. The popup window is triggered automatically, showcasing a simple implementation of interactive web elements.

## Features

- Automatic popup window on page load
- Responsive design using CSS
- Minimalistic and easy-to-understand code

## Usage

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/automatic-popup-window.git
   ```

2. Open the `index.html` file in your web browser.

3. Experience the automatic popup window on page load.

## Code Structure
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Automatic Popup</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
    <!-- Stylesheets -->
    <style media="screen">
        /* Reset and base styles */
        *,
        *:before,
        *:after {
            padding: 0;
            margin: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
        }

        .popup {
            background-color: #ffffff;
            width: 420px;
            padding: 30px 40px;
            position: absolute;
            transform: translate(-50%,-50%);
            left: 50%;
            top: 50%;
            border-radius: 8px;
            font-family: "Poppins", sans-serif;
            display: none; 
            text-align: center;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
        }

        .popup button {
            display: block;
            margin: 0 0 20px auto;
            background-color: transparent;
            font-size: 30px;
            color: #ffffff;
            background: #03549a;
            border-radius: 100%;
            width: 40px;
            height: 40px;
            border: none;
            outline: none;
            cursor: pointer;
        }

        .popup button:hover {
            background-color: #02416e;
        }

        .popup h2 {
            margin-top: -20px;
            color: #333333;
        }

        .popup p {
            font-size: 14px;
            text-align: justify;
            margin: 20px 0;
            line-height: 25px;
            color: #666666;
        }

        a {
            display: block;
            width: 150px;
            position: relative;
            margin: 10px auto;
            text-align: center;
            background-color: #0f72e5;
            border-radius: 20px;
            color: #ffffff;
            text-decoration: none;
            padding: 8px 0;
        }

        a:hover {
            background-color: #0c5ec1;
        }

        /* Media Query for Responsiveness */
        @media screen and (max-width: 480px) {
            .popup {
                width: 90%;
                padding: 20px;
            }

            .popup button {
                font-size: 24px;
                width: 30px;
                height: 30px;
            }

            .popup h2 {
                font-size: 24px;
            }

            .popup p {
                font-size: 12px;
                line-height: 20px;
            }

            a {
                width: 120px;
                font-size: 12px;
            }
        }
    </style>
</head>
<body>
    <div class="popup">
        <button id="close">&times;</button>
        <h2>Automatic Pop-Up</h2>
        <p>Join the CheggNx community for access to valuable study resources, Chegg solutions, and engaging academic discussions. Whether you're a student seeking help or an enthusiast looking to enhance your knowledge, CheggNx is the place to be!
        </p>
        <a href="https://t.me/cheggnx">Let's Go</a>
    </div>

    <!-- Script -->
    <script type="text/javascript">
        window.addEventListener("load", function(){
            setTimeout(function() {
                document.querySelector(".popup").style.display = "block";
            }, 2000);
        });

        document.querySelector("#close").addEventListener("click", function(){
            document.querySelector(".popup").style.display = "none";
        });
    </script>
</body>
</html>

```
- `index.html`: The main HTML file containing the structure of the webpage.
- `styles.css`: The CSS file for styling the webpage and the popup window.
- `script.js`: The JavaScript file for handling the automatic popup functionality.

## Customization

Feel free to customize the content, styling, and behavior of the popup window according to your preferences. You can modify the HTML, CSS, and JavaScript files to suit your needs.

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE.md).

## Contact

If you have any questions or suggestions, feel free to reach out to [MUSTKEEM324@GMIAL.COM].

Happy coding!
