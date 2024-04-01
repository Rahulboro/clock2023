# Clock Project

Welcome to the Clock Project repository! This project showcases a digital clock implemented using HTML, CSS, and JavaScript. The clock dynamically displays the current time and features a responsive design for seamless user experience across various devices.

## Features

- **Dynamic Time Display**: The clock updates in real-time to accurately reflect the current time.
- **Responsive Design**: The project is built with responsiveness in mind, ensuring optimal viewing experience on different screen sizes.

## Demo

Explore the live demo of the clock project [here](link_to_demo).

## Screenshots

Witness the elegant simplicity of the clock project through the following screenshot:

![Clock Screenshot](clock_screenshot.png)

## How to Use

To leverage the clock project's functionality:

1. **Clone Repository**: Clone this repository to your local machine.
2. **Open HTML File**: Open the `index.html` file in a modern web browser.
3. **Enjoy**: Witness the clock display the current time seamlessly.

## Project Details

Dive deeper into the intricacies of the clock project:

### Technologies Used

- **HTML**: Provides the structure and content of the clock interface.
- **CSS**: Styles the clock interface to enhance visual appeal and usability.
- **JavaScript**: Powers the dynamic functionality of the clock, ensuring real-time updates.

### Project Structure

- `index.html`: Main HTML file providing the structure of the clock interface.
- `styles.css`: Cascading Style Sheets defining the aesthetic presentation of the clock.
- `script.js`: JavaScript file containing the logic for updating and displaying the current time.

### JavaScript Functions

Explore the core JavaScript function responsible for updating the clock display:

#### `updateTime()`

```javascript
setInterval(() => {
  d = new Date();
  htime = d.getHours();
  mtime = d.getMinutes();
  stime = d.getSeconds();
  hrotation = 30 * htime + mtime / 2;
  mrotation = 6 * mtime;
  srotation = 6 * stime;

  hour.style.transform = `rotate(${hrotation}deg)`;
  minute.style.transform = `rotate(${mrotation}deg)`;
  second.style.transform = `rotate(${srotation}deg)`;
}, 1000);
```

### CSS Styling

Delve into the CSS styling defining the visual elegance of the clock:

#### `.clock`

```css
.clock-container {
  position: relative;
  background-color: rgb(178, 120, 43);
  height: 50vw;
  width: 50vw;
  border: 2px solid red;
  background: url(./asset/clock1f.png) no-repeat;
  background-size: 100%;
  margin: auto;
}
#hour,
#minute,
#second {
  position: absolute;
  background: #000;
  background: black;
  border-radius: 10px;
}
#hour {
  width: 1%;
  height: 15%;
  top: 35%;
  left: 49.4%;
  opacity: 0.9;
  transform-origin: bottom;
}
#minute {
  width: 1%;
  height: 21%;
  top: 29%;
  left: 49.4%;
  opacity: 0.9;
  transform-origin: bottom;
}
#second {
  width: 1%;
  height: 23%;
  top: 27%;
  left: 49.4%;
  opacity: 0.9;
  transform-origin: bottom;
}
```
