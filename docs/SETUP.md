# Setup Guide

## Prerequisites

- Node.js (v18 or higher)
- npm (v10 or higher)
- Angular CLI (v21.2.6)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mostafa-SAID7/lead-geny-landing.git
   cd lead-geny-landing
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm start
   ```

4. **Open browser**
   Navigate to `http://localhost:4200/`

## Development

### Running the app
```bash
npm start
```

### Building for production
```bash
npm run build
```

### Running tests
```bash
npm test
```

### Code generation
```bash
ng generate component component-name
ng generate service service-name
ng generate module module-name
```

## Troubleshooting

### Port already in use
```bash
ng serve --port 4201
```

### Clear cache
```bash
rm -rf node_modules package-lock.json
npm install
```

### Build errors
Ensure you're using the correct Node.js version:
```bash
node --version  # Should be v18+
```
