# Use public ECR image as base
FROM public.ecr.aws/lambda/python:3.12

# Copy the application files to the container
COPY . /var/task

# Install any necessary dependencies
RUN pip install -r requirements.txt

# Set the CMD to your handler (could also be done as a parameter override outside of the Dockerfile)
CMD ["main.handler"]
