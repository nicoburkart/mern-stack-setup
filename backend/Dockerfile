# Use a lighter version of Node as a parent image
FROM mhart/alpine-node:14.17
# Set the working directory to /backend
WORKDIR /backend
# copy package.json into the container at /backend
COPY package*.json /backend/
# install dependencies
RUN npm install
# Copy the current directory contents into the container at /backend
COPY . /backend/
# Make port 80 available to the world outside this container
EXPOSE 8080
# Run the app when the container launches
CMD ["npm", "start"]
