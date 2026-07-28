# Jateow 

Jateow is a job Application Tracker, client side web application for tracking job applications. Built as a single HTML file with built in data persistence using localStorage.

## Overview

Jateow is a job application tracking tool that allows users to add, edit, delete, and filter job applications. All data is stored locally in the browser, requiring no server or database setup.

## Features

- Add new job applications with company, role, date applied, status, and optional notes
- Edit existing applications
- Delete individual applications or batch delete multiple entries
- Filter applications by status (Applied, Interview, Offer, Rejected, Saved)
- Search applications by company name or role
- Sort applications by date (newest/oldest) or company name (A-Z)
- Dark/light theme toggle with persistent preference
- Responsive design for desktop and mobile devices
- Statistics dashboard showing total applications and counts by status
- Batch selection mode for bulk operations

## Technologies

- HTML5
- CSS3 (custom properties for theming, responsive grid/flexbox layouts)
- Vanilla JavaScript (ES6)
- localStorage for data persistence



## File Structure

```
index.html          # Single-file application (HTML, CSS, and JavaScript)
assets/
  images/
    Jateow_Logo.jpg
```

## Installation & Usage

1. Download or clone the `index.html` file.
2. (Optional) Place image at `assets/images/Jateow_Logo.jpg`.
3. Open `index.html` in any web browser.
4. The application is ready to use. All data is saved automatically to your browser's localStorage.


## Data Storage

All application data is stored in the browser's localStorage under the key `jobAppTracker_data`. The theme preference is stored under `jobAppTracker_theme`. Data persists across browser sessions and is not sent to any external server.


## Configuration

### Theme Preference

The theme preference is stored in localStorage under the key `jobAppTracker_theme`. Valid values are `light` and `dark`. The default is `light`.

### Data Storage Key

The application data is stored in localStorage under the key `jobAppTracker_data`. This key can be modified in the JavaScript source if needed.

### Color Theme

CSS custom properties are defined in the `:root` selector and the `[data-theme="dark"]` selector. Modify these variables to change the application's color scheme.

## Limitations

- Data is stored locally in the browser. Clearing browser data will remove all applications.
- No export/import functionality for application data.
- No user authentication or multi-device sync.
- Date filtering uses local system date.
