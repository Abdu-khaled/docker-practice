## Use node:20 as the base image
FROM node:20

# Set working directory
WORKDIR /app

# Copy package files 
COPY package*.json ./

# Install aLL dependencies 
RUN npm install

# Copy the rest of the source
COPY . .

# Build the app
RUN npm run build

# Expose port 3000
EXPOSE 3000

# Start the app
CMD ["npm", "run", "start"]