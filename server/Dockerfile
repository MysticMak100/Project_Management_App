# Use the official Node.js image as the base image
FROM node:16-buster

# Set the working directory in the container to /app
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package.json package-lock.json ./

# Install dependencies
RUN npm ci

# Copy the rest of the application files to the container
COPY . .

# Expose port 5000 to the host
EXPOSE 5000

# Command to run the application
CMD ["npm", "run", "start"]
