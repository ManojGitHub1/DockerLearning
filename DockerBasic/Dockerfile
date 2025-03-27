FROM node:19-alpine  

# Create app directory
WORKDIR /app

# Copy package.json and package-lock.json first
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose port (optional, useful if you're using Express or similar frameworks)
# EXPOSE 3000

# Run the application
CMD ["node", "index.js"]
