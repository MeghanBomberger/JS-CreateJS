# Build a Game with CreateJS

## Setup

### Installation

Run the `npm install` command from the root folder of the cloned project. This will install all dependencies.

### Verify Setup

To verify that everything is set up correctly, run the `npm run test` command. This  should show you the failing tests. This is good! We'll be fixing these tests once we jump into the build step.

Every time you want to check your work locally you can type the `npm run test` command, and it will report the status of every test in that module.

### Previewing Your Work

To see your changes in the browser, you can run the `npm start` command. This will open a browser and where you should be able to see your landing page.

## Module 01 - Main Game Loop

### 1.1 - Reference an External Script

`@external-script`, open `index.html` and add a `script` tag that references the CreateJS on the CreateJS CDN.

Next, add a `script` tag for the `app.js` file.

### 1.2 - Listen for DOMContentLoaded

`@listen-domcontentloaded`, open `app.js` and add an event listener to the `document`. Listen to the `DOMContentLoaded` event. The event handler should be an anonymous function.

### 1.3 - Keycode Constants

`@keycode-constants`, at the top of the event handler anonymous function declare four constants called `KEYCODE_LEFT`, `KEYCODE_UP`, `KEYCODE_RIGHT`, and `KEYCODE_DOWN`. Assign them the values 37, 38, 39 and 40 to each constant respectively.

### 1.4 - Create a Stage

`@create-stage`, below the key code constants assign a constant called `stage` the value `new createjs Stage`. Make sure that you have the proper ID.

### 1.5 - Create a Shape

`@shio-shape`, below the `stage` constant, assign a constant called `ship` the value `new createjs Shape`.

### 1.6 - Draw a Ship Shape

`@draw-ship`, on the `graphics` layer of the `ship` shape draw a white ship with the following points (0, 0), (30, 15), (0, 30), (7.5, 15), (0, 0).

### 1.7 - Add a Shape to the Stage

`@ship-addchild`, add the `ship` Shape to `stage`.

### 1.8 - Ticker Event Listener

`@ticker-event-listener`, using the `createjs.Ticker` object's `on` method, register a handler for the "tick" event. The handler function should be an anonymous function that updates the `stage`.

### 1.9 - Ticker FPS

`@Ticker-fps`, use the `createjs.Ticker` object and `setFPS()` to set the frames per second to 30.

### 1.10 - Keyboard Listener

`@keyboard-listener`, listen for when a user presses a key down. The handler should be called an anonymous function with an `event` argument.

### 1.11 - Switch Statement

`@switch-statement`, create a new switch statement and test the `event.keyCode`.

### 1.12 - Left Key

`@left-key`, create a case for `KEYCODE_LEFT` that moves the ship left at the rate of 15 pixels. Then `break` out of this case.

### 1.13 - Up Key

`@up-key`, create a case for `KEYCODE_UP` that moves the ship up at the rate of 15 pixels. Then `break` out of this case.

### 1.14 - Right Key

`@up-key`, create a case for `KEYCODE_RIGHT` that moves the ship right at the rate of 15 pixels. Then `break` out of this case.

### 1.15 - Down Key

`@down-key`, create a case for `KEYCODE_DOWN` that moves the ship right at the rate of 15 pixels. Then `break` out of this case.
