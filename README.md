# Quiz Management System

A real-time quiz buzzer management system built with Node.js and WebSockets. Designed for live quiz competitions with multiple teams, a host control panel, and a projector display.

## Project Structure

```
├── server.js              # Node.js server (HTTP + WebSocket)
├── package.json           # Project dependencies
├── public/                # Static files served to clients
│   ├── index.html         # Host control panel
│   ├── display.html       # Projector/audience display
│   ├── buzzer.html        # Team buzzer interface
│   ├── team1.html         # Team 1 redirect page
│   ├── team2.html         # Team 2 redirect page
│   ├── team3.html         # Team 3 redirect page
│   ├── team4.html         # Team 4 redirect page
│   ├── css/
│   │   ├── host.css       # Styles for host control panel
│   │   └── display.css    # Styles for projector display
│   └── js/
│       └── questions.js   # Question bank for all rounds
├── LICENSE
└── README.md
```

## Features

- **4 Quiz Rounds** with different formats (MCQ, category-based, rapid fire, buzzer round)
- **Real-time Buzzer System** via WebSocket communication
- **Host Control Panel** for managing rounds, scores, and buzzer control
- **Projector Display** for showing questions and scores to the audience
- **Team Buzzer Pages** accessible from any device on the same network
- **Tiebreaker Support** for resolving tied scores

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v10.0.0 or higher)

### Installation

```bash
npm install
```

### Running the Server

```bash
npm start
```

The server will start on port 3000 (or the port specified by the `PORT` environment variable). The console will display URLs for:

- **Host Panel** — Main quiz master interface
- **Display** — Projector/audience screen
- **Team Buzzers** — Individual team buzzer pages

All devices must be connected to the same network.

## Usage

1. Open the **Host Panel** on the quiz master's device
2. Open the **Display** page on the projector
3. Share the **Team Buzzer** links with each team
4. Configure team names and start the quiz from the Host Panel

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
