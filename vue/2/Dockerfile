# Use official Node.js 14 image (good for Vue 2 projects)
FROM node:14

# Set working directory
WORKDIR /app

# Copy package files first (for caching)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the app
COPY . .

# Expose the port Vue dev server listens on
EXPOSE 8080

# Start Vue dev server
CMD ["npm", "run", "serve"]
