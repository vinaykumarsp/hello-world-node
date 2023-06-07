# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory inside the container
WORKDIR /node-hello

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the application dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose the port on which the application will run
EXPOSE 3000

# Start the Node.js application
CMD ["node", "index.js"]

