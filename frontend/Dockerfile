FROM node:18-alpine

WORKDIR /app

# Set Node memory limit
ENV NODE_OPTIONS="--max-old-space-size=4096"

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy source directory
COPY src/ src/

# Copy public directory
COPY public/ public/

EXPOSE 3000

CMD ["npm", "start"] 