# Plinko Gambling Game

A browser-based gambling game inspired by **Stake.com's Plinko**, where users drop a ball into a board filled with obstacles. The ball bounces and falls through randomized paths, ultimately landing in a slot that determines the payout multiplier.

## Gameplay Overview

- Click "Drop Ball" to start.
- The ball travels downward, bouncing off pegs using realistic physics and collision mechanics.
- It lands in one of the final multipliers at the bottom.
- Your `winnings = Bet × Multiplier` from the slot where the ball lands.

## Features

-  Interactive UI with smooth ball animations
-  Collision mechanics for realistic bouncing behavior
-  Customizable multipliers and slot configurations
-  Unlimited plays with each click simulating a new drop
-  Calculates and displays final winnings based on hit multiplier  

## Tech Stack

- **Frontend**: React.js, Node.js, HTML, CSS, JavaScript `(Canvas or DOM-based)`
- **Physics**: Custom collision detection and response for bouncing logic
- **Animations**: JavaScript animation loop `requestAnimationFrame`

## Project Structure

```bash
├── backend/              # All backend logic here     
│   ├── src/        
│   │    ├── index.ts     
│   │    └── outcomes.ts   
├── frontend/             # All frontend logic here       
│   ├── src/        
│   │    ├── components/  
│   │    ├── game/
│   │    ├── pages/
│   │    ├── utils/
│   │    └── App.tsx
├── version-1             # Basic version of the application
└── README.md             # README.md file
```

## Installation

1. **Clone the Repository**

```bash
git clone [repository-url]
cd Plinkoo
```

2. **Install the backend dependencies**

```bash
cd backend
npm install
```

3. **Install the frontend depedencies**

```bash
cd frontend
npm install
```

4. **Start the backend server**

```bash
cd backend
npm run dev
```

5. **Start the frontend application**

```bash
cd frontend
npm run dev
```

6. **Additionally you can also use the HTML version of this application by navigating to `version-1`**

```bash
cd vesrion-1
start index.html
```

## Contributing

We welcome contributions from the community! Whether you're interested in improving features, fixing bugs, or adding new functionality, your input is valuable. Feel free to reach out to us with your ideas and suggestions.

## License
This project is licensed under the MIT License - see the LICENSE file for details.