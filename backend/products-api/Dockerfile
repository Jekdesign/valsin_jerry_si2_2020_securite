# Use a lighter version of Node as a parent image
FROM mhart/alpine-node:12

# Set the working directory to /api
WORKDIR /products-api/

# Copy the current directory contents into the container at /api
COPY . /products-api/

# install dependencies
RUN npm install

# Make port available to the world outside this container
EXPOSE 3002

# Run the app when the container launches
CMD [ "npm", "start" ]