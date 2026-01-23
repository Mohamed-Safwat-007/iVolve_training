Lab 4: Run Java Spring Boot App in a Container

• Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-1.git

    git clone https://github.com/Ibrahim-Adel15/Docker-1.git
    cd Docker-1


<img width="950" height="314" alt="image" src="https://github.com/user-attachments/assets/06f41637-b046-4e99-9207-0700277fb01e" />


• Build the application.

    mvn clean package


<img width="819" height="652" alt="image" src="https://github.com/user-attachments/assets/e69bd0e5-2e09-42ee-a80c-54a992175f50" />


• Write Dockerfile.

    nano Dockerfile


<img width="884" height="196" alt="image" src="https://github.com/user-attachments/assets/5901912f-259d-4f93-a752-b6c9af434b4d" />


• Build app2 Image (Note the image size).

    docker build -t app2 .

    docker images


<img width="821" height="648" alt="image" src="https://github.com/user-attachments/assets/3607abba-d7cc-412a-8eca-fc1ffa9816f2" />


• Run container2 from app2 image.

    docker run -d --name container2 -p 8080:8080 app2

    docker ps


<img width="822" height="258" alt="image" src="https://github.com/user-attachments/assets/1dd2bdc0-c8a3-4f74-8da7-afc6858ee647" />


• Test the application.


<img width="810" height="231" alt="image" src="https://github.com/user-attachments/assets/0dfa856e-89d2-46a2-8c00-26344884ab38" />


• Stop and delete the container.

    docker stop container2

    docker rm container2


<img width="841" height="224" alt="image" src="https://github.com/user-attachments/assets/b3eb8420-1b2d-4267-9fbc-c4f880250772" />
