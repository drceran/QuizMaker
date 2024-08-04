# Use the official Node.js image.
FROM node:18

# Set the working directory
WORKDIR /frontend

# Copy package.json
COPY package.json  ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

COPY .next .next


# Expose port 3000
EXPOSE 3000

# Start the application
CMD ["npm", "run" ,"start"]
