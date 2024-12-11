# Docker Hello Captain

This repository demonstrates the creation of a basic Docker file that prints the '**Hello Captain**' message in the terminal on run before exiting.

## Following steps can be followed to build and run the Docker container:

1. **Create a Dockerfile** without any extensions and write the following code in it:

    ```bash
    FROM alpine:latest
    LABEL maintainer="Rahul Parihar"
    LABEL email="rahulaauji71@gmail.com"
    CMD [ "echo", "Hello Captain" ]
    ```
2.	**Save the file as Dockerfile.**

3.	**Build the Docker image using the following command:**

    ```bash
    docker build -t hello-captain .
    ```

4.	Run the Docker container to print the “Hello Captain” message:

    ```bash
    docker run hello-captain
    ```

5.	Output: The following message will be printed in the terminal:

    ```bash
    Hello Captain
    ```
## You can also Pull the repository from following URL.
### Project URL : You can use this url <a href="https://github.com/rahulaauji-30/docker-hello-captain.git">here</a>
## Notes:<br>
	•	This Dockerfile uses the alpine:latest image as a base.<br>
	•	The CMD instruction tells Docker to print “Hello Captain” when the container runs.
	•	The container will exit after printing the message.