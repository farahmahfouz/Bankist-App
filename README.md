# Bankist App

## Overview
Bankist is a minimalist banking application that simulates basic banking operations. It's a front-end focused project built with vanilla JavaScript, demonstrating modern JavaScript features and DOM manipulation.

## Features
- **User Authentication**: Secure login system with username and PIN
- **Transaction History**: View detailed transaction history with dates
- **Real-time Balance**: Automatic balance calculation and display
- **Money Transfer**: Transfer money between existing accounts
- **Loan Request**: Request loans based on account history
- **Account Closure**: Option to close existing accounts
- **Auto Logout**: Timer-based automatic logout system
- **Transaction Sorting**: Ability to sort transactions by amount
- **Internationalization**: Support for different number and date formats

## Installation

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Basic understanding of command line interface
- Git (optional, for cloning)
- Code editor (VS Code, Sublime Text, or similar)

### Installation Methods

#### Method 1: Direct Download
1. Download the project files
   ```
   - index.html
   - style.css
   - script.js
   ```
2. Create a new folder for the project
3. Place all downloaded files in the folder
4. Open `index.html` in your browser

#### Method 2: Using Git
1. Open your terminal
2. Clone the repository:
   ```bash
   git clone [https://github.com/farahmahfouz/Bankist-App.git]
   cd bankist
   ```
3. Open `index.html` in your browser

#### Method 3: Using Local Development Server (Recommended)
1. Install Node.js from [nodejs.org](https://nodejs.org)
2. Install a development server like `live-server`:
   ```bash
   npm install -g live-server
   ```
3. Navigate to the project directory:
   ```bash
   cd bankist
   ```
4. Start the server:
   ```bash
   live-server
   ```
5. The application will automatically open in your default browser

### Development Setup
For those who want to modify the code:
1. Install a code editor (VS Code recommended)
2. Install helpful extensions:
   - Live Server
   - JavaScript (ES6) code snippets
   - Prettier - Code formatter
3. Enable auto-save and formatting on save in your editor settings

## Demo Accounts
```
Account 1:
- Username: js (Jonas Schmedtmann)
- PIN: 1111

Account 2:
- Username: jd (Jessica Davis)
- PIN: 2222
```

## Project Structure
```
bankist/
├── index.html          # Main HTML file containing the app structure
├── style.css          # Styling and layout definitions
└── script.js          # Application logic and functionality
```

## Technical Details
### Key JavaScript Features Used
- ES6+ Syntax
- Array Methods (map, filter, reduce, find, some)
- DOM Manipulation
- Event Handlers
- Internationalization API
- Date and Time Operations
- Timer Functions

### Functions Overview
- `startTimer()`: Manages the auto-logout functionality
- `formatMovementDate()`: Formats transaction dates
- `formatCur()`: Handles currency formatting
- `displayMovements()`: Renders transaction history
- `calcDisplayBalance()`: Calculates and displays current balance
- `calcDisplaySummary()`: Computes and shows account statistics
- `createUsernames()`: Generates usernames from full names
- `updateUI()`: Updates the user interface

## Getting Started
1. Clone the repository
2. Open `index.html` in your browser
3. Log in using one of the demo accounts
4. Explore the features:
   - View your transaction history
   - Transfer money to other accounts
   - Request a loan
   - Sort transactions by amount
   - Close your account

## Notes
- The app uses browser localStorage to maintain data during the session
- All monetary values are formatted according to the user's locale
- The automatic logout timer resets with each operation
- Loan requests are granted if there's at least one deposit >= 10% of the requested amount

## Troubleshooting
- If the page doesn't load properly, clear your browser cache
- Make sure all files are in the same directory
- Check your browser's console for any JavaScript errors
- Ensure you're using a modern browser with ES6+ support

## Security Note
This is a demo project and does not implement actual security measures. In a production environment, proper authentication, data encryption, and secure communication protocols would be necessary.
