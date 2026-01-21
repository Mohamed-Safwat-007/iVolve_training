Lab 6: Managing Docker Environment Variables Across Build and Runtime

• Clone the Application Code https://github.com/Ibrahim-Adel15/Docker-3.git

git clone https://github.com/Ibrahim-Adel15/Docker-3.git

cd Docker-3

<img width="799" height="280" alt="image" src="https://github.com/user-attachments/assets/b1742949-d24e-4d52-807f-b767a3498e38" />

• Write Dockerfile

nano Dockerfile

ls

<img width="868" height="215" alt="image" src="https://github.com/user-attachments/assets/7d738c8d-41cc-49cc-8092-5368b9d60b6a" />

• Build Docker Image

docker build -t env-app .

docker images


<img width="820" height="666" alt="image" src="https://github.com/user-attachments/assets/db6a60ba-8cd9-43b1-adf2-cb50e0115401" />

• Run 3 containers and set both environment variables (APP_MODE & APP_REGION) as
following:

i. (development, us-east) as variables in the command when run docker container

docker run -d --name dev-container -p 8081:8080 -e APP_MODE=development -e APP_REGION=us-east env-app


<img width="864" height="187" alt="image" src="https://github.com/user-attachments/assets/76eb8379-7580-48d8-999a-1eb27ce38d35" />


ii. (staging, us-west) in a separate file and pass the file name in the command

nano staging.env

    APP_MODE=staging
    
    APP_REGION=us-west

docker run -d --name staging-container -p 8082:8080 --env-file staging.env env-app

<img width="892" height="258" alt="image" src="https://github.com/user-attachments/assets/b273f81c-e49a-4ec4-8c89-e4a0912c08ff" />

iii. (production, canada-west) in the Dockerfile

docker run -d --name prod-container -p 8083:8080 env-app

<img width="888" height="206" alt="image" src="https://github.com/user-attachments/assets/4e378d4c-550f-4349-89f6-f9ec075bc517" />

docker ps
<img width="1311" height="178" alt="image" src="https://github.com/user-attachments/assets/98af53c6-7c06-4b82-a8e2-398f12755cb0" />
