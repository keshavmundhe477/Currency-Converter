# Currency Converter

This is a simple Currency Converter application built using HTML, CSS, and JavaScript. The app allows users to convert an amount from one currency to another using real-time exchange rates.

## Demo

You can use the currency converter [here](https://keshavmundhe477.github.io/Currency-Converter/).

## GitHub Repository

You can view the source code and contribute to the project [here](https://github.com/keshavmundhe477/Currency-Converter).

## Features

- Users can enter an amount to convert.
- Select the currencies to convert from and to.
- Fetches real-time exchange rates using an external API.
- Displays the converted amount and exchange rate.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/keshavmundhe477/Currency-Converter.git
    ```
2. Navigate to the project directory:
    ```sh
    cd Currency-Converter
    ```

## Usage

1. Open `index.html` in your web browser:
    ```sh
    open index.html
    ```

2. Enter the amount you want to convert.
3. Select the currencies to convert from and to.
4. Click on "Get Exchange Rate" to see the converted amount.

## Code Overview

### index.html

This file contains the structure of the currency converter. It includes input fields for the amount, dropdown lists for selecting currencies, and a section to display the exchange rate.

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Currency Converter App in JavaScript</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- FontAweome CDN Link for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"/>
  </head>
  <body>
    <div class="wrapper">
      <header>Currency Converter</header>
      <form action="#">
        <div class="amount">
          <p>Enter Amount</p>
          <input type="text" value="1">
        </div>
        <div class="drop-list">
          <div class="from">
            <p>From</p>
            <div class="select-box">
              <img src="https://flagcdn.com/48x36/us.png" alt="flag">
              <select> <!-- Options tag are inserted from JavaScript --> </select>
            </div>
          </div>
          <div class="icon"><i class="fas fa-exchange-alt"></i></div>
          <div class="to">
            <p>To</p>
            <div class="select-box">
              <img src="https://flagcdn.com/48x36/np.png" alt="flag">
              <select> <!-- Options tag are inserted from JavaScript --> </select>
            </div>
          </div>
        </div>
        <div class="exchange-rate">Getting exchange rate...</div>
        <button>Get Exchange Rate</button>
      </form>
    </div>
    <script src="js/country-list.js"></script>
    <script src="js/script.js"></script>
  </body>
</html>
