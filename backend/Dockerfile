FROM node:18

WORKDIR /app

# Clear any previous node_modules to avoid conflicts
RUN rm -rf node_modules

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies and rebuild native modules
RUN npm install --build-from-source

# Copy the rest of the application
COPY . .

EXPOSE 8080
CMD ["node", "server.js"]
