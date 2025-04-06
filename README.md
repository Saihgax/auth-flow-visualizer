# Authentication Flow Visualizer

This project provides a visual representation of various authentication flows to help new hires understand identity concepts. It includes a Golang backend that models authentication processes and a web-based frontend for interactive visualization.

## Directory Structure

```
auth-flow-visualizer/
├── cmd/
│   └── server/
│       └── main.go              # Application entry point
├── internal/
│   ├── api/
│   │   ├── handlers.go          # HTTP handlers
│   │   ├── middleware.go        # API middleware
│   │   └── routes.go            # API route definitions
│   ├── auth/
│   │   ├── models.go            # Authentication data models
│   │   ├── flows.go             # Auth flow implementations
│   │   └── simulator.go         # Simulation logic
│   └── config/
│       └── config.go            # Application configuration
├── web/
│   ├── static/
│   │   ├── css/
│   │   │   └── styles.css       # Custom styling
│   │   ├── js/
│   │   │   ├── visualizer.js    # Visualization logic
│   │   │   ├── controllers.js   # Playback controls
│   │   │   └── flows.js         # Flow-specific logic
│   │   └── images/              # Icons and assets
│   ├── templates/
│   │   ├── index.html           # Main application page
│   │   └── flows/               # Flow-specific templates
│   └── index.go                 # Web asset handler
├── Makefile                     # Build automation
├── go.mod                       # Go module definition
├── go.sum                       # Go dependency lockfile
└── README.md                    # Project documentation
```

## Core Components

1. **Authentication Flow Models**: Defines entities and processes in various authentication methods
2. **Flow Simulator**: Generates step-by-step state changes during authentication
3. **API Layer**: Serves flow data to the frontend
4. **Visualization Engine**: Renders the authentication flow with play/pause controls