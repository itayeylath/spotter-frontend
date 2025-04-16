# Spotter Frontend

## Prerequisites

- Node.js (v18 or later)
- npm or yarn
- Docker and Docker Compose (for containerized development)
- Expo Go app (for testing on mobile devices)

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
- `npm run build` - Build the app

## Deployment

### Web Deployment

1. Build the web version:

   ```bash
   npm run build:web
   ```

2. Deploy the contents of the `web-build` directory to your hosting service.

### Mobile Deployment

1. Configure the app.json with your app details
2. Build the app:

   ```bash
   expo build:android
   expo build:ios
   ```

3. Submit to respective app stores

## Contributing

1. Create a new branch for your feature
2. Make your changes
3. Submit a pull request
4. Wait for review and approval

## License

[Your License Here]
