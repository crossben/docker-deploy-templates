# Use official Node.js 16 image
FROM node:16

# Set working directory
WORKDIR /app

# Copy package files first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy app source code
COPY . .

# Expose Express default port
EXPOSE 3000

# Start Express server
CMD ["npm", "start"]
