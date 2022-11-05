# select a base image
FROM node:alpine

# create an application directory
RUN mkdir frontend

# copy the app package 
COPY . ./frontend

# choose the main application directory
WORKDIR ./frontend

# Install node package
RUN npm install

# Build the app 
RUN npm run build 

# expose port 
EXPOSE 3000

# start the app 
CMD ["npm" , "start"]
