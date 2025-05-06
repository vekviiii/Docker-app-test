# Use an official Node.js image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json first
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose the port Vite runs on (default: 5173)
EXPOSE 5173

# Start Vite instead of react-scripts
CMD ["npm", "run", "dev"]