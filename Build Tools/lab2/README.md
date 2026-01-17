Lab 2: Building and Packaging Java Applications with maven


• Install maven.
  sudo dnf install maven


<img width="1401" height="703" alt="image" src="https://github.com/user-attachments/assets/f2617745-f2e0-4bdd-b9a0-b490cba39b16" />


• Clone source code https://github.com/Ibrahim-Adel15/build2.git

  git clone https://github.com/Ibrahim-Adel15/build2.git
  
  cd build2


<img width="1097" height="252" alt="image" src="https://github.com/user-attachments/assets/0ae088b4-18b1-4e3c-a9c9-c860f7386fba" />


• Run Unit test.

  mvn test


<img width="1068" height="643" alt="image" src="https://github.com/user-attachments/assets/0c463e02-4590-48c1-bf16-0e323368e687" />


• Build App [ generate artifact in target/ hello-ivolve-1.0-SNAPSHOT.jar ].

mvn package


<img width="1105" height="691" alt="image" src="https://github.com/user-attachments/assets/1071f80f-72e5-4c0f-af80-da840d5dea51" />


• Run App.

  java -jar target/hello-ivolve-1.0-SNAPSHOT.jar

<img width="1271" height="245" alt="image" src="https://github.com/user-attachments/assets/f4c5e32f-91a8-4e78-90d4-18c3e114717d" />
