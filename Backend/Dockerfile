# Use Node.js official image
FROM node:18

# Create app directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy app source code
COPY . .

# Expose the port (matching server.js port or env PORT)
EXPOSE 3801

# Start the server
CMD ["node", "server.js"]


