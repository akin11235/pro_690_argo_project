# Use the official Node.js Alpine image
FROM node:18-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json for dependency installation
COPY package*.json ./

# Install Angular CLI globally and application dependencies
RUN npm install -g @angular/cli && npm install

# Copy application source code
COPY . .

# Expose the app's port
EXPOSE 4200

# Start the Angular application
CMD ["ng", "serve", "--host", "0.0.0.0"]