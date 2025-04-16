# Spotter Frontend

## Prerequisites

- Node.js (v18 or later)
- npm or yarn
- Docker and Docker Compose (for containerized development)
- Expo Go app (for testing on mobile devices)
- iOS Simulator (for iOS development)
- Android Studio (for Android development)

## Getting Started

### Local Development

1. Clone the repository:

   ```bash
   git clone [repository-url]
   cd spotter-frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm start
   ```

4. Use the Expo Go app on your mobile device to scan the QR code, or press:
   - `w` to open in web browser
   - `i` to open in iOS simulator
   - `a` to open in Android emulator

### Docker Development

1. Build and start the container:

   ```bash
   docker-compose up --build
   ```

2. Access the development server:
   - Web: http://localhost:19006
   - Expo DevTools: http://localhost:19002

## Development Guidelines

### Code Style

- Follow TypeScript best practices
- Use functional components with hooks
- Follow the established project structure
- Write meaningful commit messages

### State Management

- Use Redux for global state
- Use local state for component-specific state
- Follow Redux best practices and patterns

### Navigation

- Use React Navigation for routing
- Keep navigation logic in the navigation directory
- Use type-safe navigation with TypeScript

### UI Components

- Use React Native Paper components
- Follow Material Design guidelines
- Keep components reusable and modular

## Available Scripts

- `npm start` - Start the development server
- `npm run android` - Run on Android
- `npm run ios` - Run on iOS
- `npm run web` - Run on web
- `npm test` - Run tests
- `npm run lint` - Run ESLint

## Development Workflow

1. Start the development server:

   ```bash
   npm start
   ```

2. Choose your target platform:

   - Press `w` for web
   - Press `i` for iOS
   - Press `a` for Android
   - Scan QR code with Expo Go app for physical device

3. Make changes to your code:
   - Changes will automatically reload in the development environment
   - Hot reloading is enabled by default

## Troubleshooting

### Common Issues

1. **Metro Bundler Port Conflict**

   ```bash
   # Kill the process using port 19000
   lsof -i :19000
   kill -9 <PID>
   ```

2. **iOS Simulator Not Starting**

   - Ensure Xcode is installed
   - Open iOS Simulator manually before running the app

3. **Android Emulator Not Starting**
   - Ensure Android Studio is installed
   - Open Android Emulator manually before running the app

### Docker Issues

1. **Port Already in Use**

   ```bash
   # Stop existing containers
   docker-compose down
   # Start fresh
   docker-compose up --build
   ```

2. **Container Not Updating**
   ```bash
   # Rebuild the container
   docker-compose up --build --force-recreate
   ```

## Contributing

1. Create a new branch for your feature
2. Make your changes
3. Submit a pull request
4. Wait for review and approval

## License

[Your License Here]
