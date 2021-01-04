# Use a lighter version of Node as a parent image
FROM mhart/alpine-node:12

# Set the working directory to /api
WORKDIR /auth-api/

# Copy the current directory contents into the container at /api
COPY . /auth-api/

# install dependencies
RUN npm install

# Make port available to the world outside this container
EXPOSE 3001

# Run the app when the container launches
CMD [ "npm", "start" ]