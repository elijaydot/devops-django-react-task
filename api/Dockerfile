# select a base image
FROM python:3.9

# create an application directory
#RUN apk update \
#    && apk install -y --no-install-recommends \
#   && rm -rf /var/lib/apt/lists/*

# copy the app package 
COPY . ./api

# choose the main application directory
WORKDIR ./api

# Install requirements
RUN pip install -r requirements.txt 

# expose port 
EXPOSE 8005

# start the app 
CMD ["python", "manage.py", "runserver", "0.0.0.0:8005"]
