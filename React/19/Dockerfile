# Use official Node.js LTS image (adjust version if needed)
FROM node:20-alpine

# Set working directory inside container
WORKDIR /app

# Copy package files (this assumes user has already created a React 19 app)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app
COPY . .

# Build the React app for production (optional if using dev server)
RUN npm run build

# Expose the React development server port
EXPOSE 3000

# Start the app (change to npm run start if needed)
CMD ["npm", "start"]
