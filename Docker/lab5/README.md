Lab 5: Multi-Stage Build for a Node.js App

• Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-1.git

    cd Docker-1

<img width="901" height="167" alt="image" src="https://github.com/user-attachments/assets/08b4b352-49d7-407b-a74f-5f6fb218c0f4" />


• Write Dockerfile with Multi-stage.

    nano Dockerfile

<img width="888" height="181" alt="image" src="https://github.com/user-attachments/assets/a61dbbe6-51ff-4fad-a9ba-e01825946d93" />


• Build app3 Image (Note the image size).

    docker build -t app3 .

    docker images

<img width="808" height="650" alt="image" src="https://github.com/user-attachments/assets/0d130c77-b927-4aec-99ce-86957c16ca4e" />


• Run container3 from app3 image.

    docker run -d --name container3 -p 8080:8080 app3

    docker ps


<img width="894" height="271" alt="image" src="https://github.com/user-attachments/assets/87eae473-a66b-44cc-a31d-7abe367ff3f0" />


• Test the application.


<img width="655" height="205" alt="image" src="https://github.com/user-attachments/assets/6ae7e8f7-4083-453c-80bf-6e48b6b5b232" />


• Stop and delete the container.

    docker stop container3

    docker rm container3

<img width="871" height="221" alt="image" src="https://github.com/user-attachments/assets/de8db29e-fd1d-4d6f-8613-b2cc272d73ec" />
