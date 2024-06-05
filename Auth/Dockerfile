# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory
WORKDIR /1169_backend

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 4000

# Define environment variable for MongoDB URL
ENV MONGO_URL=mongodb://localhost:27017/

# Command to run the application
CMD ["node", "index.js"]
