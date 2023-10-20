# Use an official Node.js runtime as a parent image
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY client/package*.json ./

# Install app dependencies
RUN npm install --force

# Copy the entire React.js app to the container
COPY client ./

# Specify the port the app will run on
EXPOSE 3000

# Start the React.js app
CMD ["npm", "start"]
