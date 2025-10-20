# Use official Node.js image suited for Astro 5 (which uses Vite v6)  
FROM node:18

# Set working directory  
WORKDIR /app

# Copy package files first (cache)  
COPY package*.json ./

# Install dependencies  
RUN npm install

# Copy the rest of the source code  
COPY . .

# Expose the default port Astro dev server listens on  
EXPOSE 3000

# Run the dev server  
CMD ["npm", "run", "dev"]
