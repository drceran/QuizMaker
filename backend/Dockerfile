# Use the official Node.js image.
FROM node:18

# Set the working directory
WORKDIR /backend

# Copy package.json and package-lock.json
COPY package.json ./

# Install dependencies
RUN npm install


# Copy the rest of the application code
COPY . .

# Build the Next.js application
RUN npm run build
# Expose port 4000 (adjust if needed)
EXPOSE 4000

# Start the application
CMD ["npm","run", "start"]
