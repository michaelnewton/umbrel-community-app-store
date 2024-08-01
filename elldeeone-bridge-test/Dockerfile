# Use a Node.js base image with Debian Buster
FROM node:14-buster

# Set the working directory
WORKDIR /app

# Clone the repository (assuming Git is available on UmbrelOS)
RUN git clone https://github.com/rdugan/kaspa-stratum-bridge.git .

# Install dependencies
RUN npm install

# Expose necessary ports
EXPOSE 5555 2114

# Start the application
CMD ["node", "src/index.js"]