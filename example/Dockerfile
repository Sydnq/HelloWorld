#This tells the conatiner that Python is is the parent image
FROM python:2.7-slim

# Set the working directory(container) to /app
WORKDIR /app

#Copy the current contents of current directory into the conatiner's /app dir
ADD . /app

#Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

#make port 80 available to the world outside this container
EXPOSE 80

#Define environment variable
ENV NAME WORLD


# Run app.py when the container launches
CMD ["python", "app.py"]
