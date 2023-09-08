# Digital_Clock
# Hosted Link:-https://tulasidurga1.github.io/Digital_Clock/
### This HTML and JavaScript code creates a digital clock that displays the current time (hours, minutes, and seconds) along with AM/PM indication. Let's break down how it works:

### HTML Structure:

- The HTML document defines the basic structure of the webpage.
- It includes metadata in the <head> section, such as character encoding, compatibility settings, viewport configuration, and the page title.
- An external CSS stylesheet (style.css) is linked to apply styles to the content.
- The main content of the page is in the <body> section.
### HTML Elements:
<h2>: This element displays the title "Digital Clock."

<div class="clock">: This <div> element with the class "clock" serves as the container for the digital clock components.

- Inside the clock container, there are four <div> elements, each containing:

 <span>: This is used to display the hours, minutes, and seconds.
 <span class="text">: This displays labels for "Hours," "Minutes," and "Seconds."
<span id="ampm">: This displays the AM/PM indication.
### CSS (style.css):

- The CSS defines the styling for various elements:
- The background image of the entire page.
- Styles for the clock container and its child elements (background color, font size, text shadow, etc.).
### JavaScript (script.js):

- JavaScript is used to update the digital clock's time and display it on the webpage.

- The JavaScript code starts by selecting various HTML elements by their IDs using document.getElementById() and assigns them to variables:

- hourEl, minuteEl, secondEl, and ampmEl are used to reference the elements that will display the time components and AM/PM indication.
- The updateClock function is defined. This function performs the following tasks:

- It retrieves the current time using new Date().getHours(), new Date().getMinutes(), and new Date().getSeconds().
- It sets the initial value of the ampm variable to "AM."
- If the hour is greater than 12, it subtracts 12 from the hour and sets ampm to "PM" to handle 12-hour time format.
- It ensures that single-digit hours, minutes, and seconds are padded with a leading "0" for a consistent format.
- It updates the text content of the selected HTML elements (hourEl, minuteEl, secondEl, and ampmEl) to display the current time and AM/PM indication.
- Finally, it schedules the updateClock function to be called again after a 1000ms (1-second) delay using setTimeout(). This creates a continuous update loop for the clock.
- The updateClock function is initially called once to display the current time when the page loads.

- Overall, this code combines HTML, CSS, and JavaScript to create a visually appealing digital clock that updates in real-time. The clock displays hours, minutes, and seconds in a 12-hour format with AM/PM indication and is styled using CSS to enhance its appearance. The updateClock function continuously updates the time, creating a live clock display on the webpage.




