Lab 1: Building and Packaging Java Applications with Gradle


• Install Gradle.

      cd /opt

      sudo wget https://services.gradle.org/distributions/gradle-8.5-bin.zip

      sudo unzip gradle-8.5-bin.zip

      sudo mv gradle-8.5 gradle


<img width="728" height="608" alt="image" src="https://github.com/user-attachments/assets/a26f25bf-36d9-43d8-ba51-afabdf6f9497" />

• Clone source code https://github.com/Ibrahim-Adel15/build1.git

      git clone https://github.com/Ibrahim-Adel15/build1.git

      cd build1


<img width="692" height="237" alt="image" src="https://github.com/user-attachments/assets/4845b02c-269a-4d5d-9d07-373d6b051e77" />


• Run Unit test.

    gradle test


<img width="1126" height="647" alt="image" src="https://github.com/user-attachments/assets/5ef04784-80be-47d3-89a2-e1bac54eb118" />


• Build App [ generate artifact in build/libs/ivolve-app.jar ].

    gradle build


<img width="988" height="400" alt="image" src="https://github.com/user-attachments/assets/293d917f-e106-48ba-bed0-38d8d31de14e" />


    ls build/libs/


<img width="908" height="200" alt="image" src="https://github.com/user-attachments/assets/56c13b09-3c02-4ac9-ad28-1ee9a03f1d4f" />


• Run App.

    java -jar build/libs/ivolve-app.jar
  

  <img width="921" height="210" alt="image" src="https://github.com/user-attachments/assets/3af4cd3a-bd10-41ff-9761-95565adddb6f" />


