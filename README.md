# Digital Clock 🕰️

Welcome to the **Digital Clock** repository! 🎉 This project showcases a simple yet elegant digital clock designed for real-time time display, allowing users to view the current time effortlessly.

## Project Overview 📚

This repository contains:
- **HTML** and **CSS** structure for the clock's user interface implementation 🌐
- **JavaScript** logic for updating the clock every second 🔄
- A feature set that provides a real-time display of the current time 🕒

## Understanding the Digital Clock ⏰

The **Digital Clock** is designed to display the current time, updating every second. 

### How the Clock Works 🔄

The clock follows these steps:
1. Initializes the time display on page load.
2. Updates the displayed time every second.
3. Utilizes JavaScript functions to format and display the current time.

### Example Time Display 🕑

Here’s an example of how the clock displays the current time:
- **Current Time**: `12:45:30 PM`

## JavaScript Implementation 💻

Here’s the core JavaScript function for updating the clock:

```javascript
function updateClock() {
    const now = new Date();
    const hours = now.getHours();
    const minutes = now.getMinutes();
    const seconds = now.getSeconds();
    const ampm = hours >= 12 ? 'PM' : 'AM';

    // Format the time to be 12-hour format
    const formattedTime = `${hours % 12 || 12}:${String(minutes).padStart(2, '0')}:${String(seconds).padStart(2, '0')} ${ampm}`;

    document.getElementById("clock").innerText = formattedTime;
}

// Update the clock every second
setInterval(updateClock, 1000);

// Initialize the clock on page load
updateClock();
```

## Usage Instructions 🛠️

To run the Digital Clock:
1. Include the JavaScript file in your HTML structure.
2. Open `index.html` in your web browser to view the clock.
3. The clock will display the current time, updating every second.

## Contact Information 📞

For questions or suggestions about this project:

- **Email**: muhammadeshareeb986@gmail.com 📧
- **LinkedIn**: [Muhammad Eshareeb](https://www.linkedin.com/in/muhammadeshareeb986/) 🦸‍♂️

Happy Coding! 🎉
