Lab 3: Run Java Spring Boot App in a Container

• Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-1.git


git clone https://github.com/Ibrahim-Adel15/Docker-1.git
cd Docker-1


<img width="911" height="414" alt="image" src="https://github.com/user-attachments/assets/848a0996-9c17-4a8d-8a58-4e869bda9975" />


• Write Dockerfile.

nano Dockerfile

• Build app1 Image.

docker build -t app1 .

<img width="788" height="664" alt="image" src="https://github.com/user-attachments/assets/e8f2b350-b61f-44bf-8479-e2c52b04d25a" />


• Run container1 from app1 Image.

docker run -d --name container1 -p 8080:8080 app1

docker ps

<img width="945" height="243" alt="image" src="https://github.com/user-attachments/assets/e5004661-8491-4379-b621-e3160ef8c1d9" />


• Test the application.

<img width="1025" height="420" alt="image" src="https://github.com/user-attachments/assets/8d359847-5325-4307-b441-8d7cbb6186e9" />


• Stop and delete the container.

docker stop container1

docker rm container1

docker ps

<img width="917" height="311" alt="image" src="https://github.com/user-attachments/assets/b4a0a17b-aa38-49c5-adb7-ca1f0d1523e3" />
