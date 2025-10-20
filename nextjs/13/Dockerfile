# Use Node LTS base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Install dependencies separately to cache better
COPY package*.json ./
RUN npm install

# Copy the rest of your code
COPY . .

# Build the Next.js app this should work unless you have a custom build script
RUN npm run build

# Expose default Next.js port, ensure it matches the PORT in docker-compose.yaml if set
EXPOSE 3000

# Start the Next.js server
CMD ["npm", "start"]
