# Use official Node.js 16 image, recommended for Vue 3 projects
FROM node:16

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json (if present)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy app source code
COPY . .

# Expose Vue dev server port
EXPOSE 8080

# Start Vue dev server
CMD ["npm", "run", "serve"]
