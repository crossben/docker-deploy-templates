# Use latest Node.js LTS
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app
COPY . .

# Build the site (optional for static generation)
RUN npm run build

# Expose Astro's default dev server port
EXPOSE 4321

# Start the dev server
CMD ["npm", "run", "dev"]
