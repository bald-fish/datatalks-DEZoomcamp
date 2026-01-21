# base Docker image for build
FROM python:3.13.11-slim

# set up image by installing prerrequisites; pandas and pyarrow
RUN pip install pandas pyarrow

#set up the working directory inside the conatiner
WORKDIR /app

#copying the script to the container working dir
COPY pipeline.py pipeline.py

#define first steps when the container is ran
ENTRYPOINT [ "python", "pipeline.py"]