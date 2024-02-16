FROM node:16

# Create app directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Copy the rest of the application code to the working directory
COPY . .

# Expose port 3001 for the application
EXPOSE 3001

# Define the command to run the app
CMD [ "node", "app.js" ]
