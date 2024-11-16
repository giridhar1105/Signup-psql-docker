FROM node:18-alpine

WORKDIR /app

# Copy package.json files first (this allows Docker to cache dependencies)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
# COPY ./src ./src

# Expose the port your app will run on
EXPOSE 4000

CMD ["node", "src/index.js"]
