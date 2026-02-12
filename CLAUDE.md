# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a world clock web application built with Vue.js 3 that displays analog and digital clocks for multiple time zones. The application features:

- Real-time analog and digital clocks for local time, India (IST), and New York
- Interactive time slider that allows users to set time for all clocks
- Responsive design that works on mobile and desktop
- Smooth animations and transitions
- Clean, modern dark-themed UI with a clock-like aesthetic

## Code Structure

The entire application is contained in a single HTML file (`index.html`) that includes:
- HTML structure for the clocks and controls
- CSS styling for the visual design
- JavaScript/Vue.js code that implements the application logic

## Key Technical Details

- Uses Vue 3's Composition API (`setup()` function)
- Implements analog clocks with SVG graphics
- Uses `Intl.DateTimeFormat` for timezone calculations
- Features a slider control with 30-minute increments (0-47 steps)
- Includes time synchronization with a 1-second interval timer
- Responsive design with media queries for mobile devices

## Development Commands

Since this is a single HTML file application with no build step, there are no specific build commands needed. Simply open `index.html` in a web browser to run the application.

## How to Run

1. Open `index.html` in any modern web browser
2. The application will automatically start and display clocks for local time, India (IST), and New York
3. Use the slider to adjust time for all clocks simultaneously
4. Click "Reset to Now" to return to current time

## Key Files

- `index.html`: Main application file containing HTML, CSS, and JavaScript/Vue code

## Implementation Notes

The application uses a clever approach to handle time zones:
- It calculates the offset between different time zones using `Intl.DateTimeFormat`
- The slider works with 30-minute increments (0-47 steps representing 00:00 to 23:30)
- Analog clocks are rendered with SVG graphics
- The time synchronization is handled with a 1-second interval timer