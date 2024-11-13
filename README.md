# FedoraLambokInstallation
### How to Install Lombok for eclipse in Fedora

**Here is the few steps** 

### From Flathub
1. Go to software and install Eclipse. 

![image](https://github.com/user-attachments/assets/5c52174d-6b15-4835-ac1a-bca4612b3189)
2. Once it's install don't open eclipse!
3. Go to this path
`/var/lib/flatpak/app/org.eclipse.Java/x86_64/stable/78f0828e03014f9b070ccefff48c738f5aac15ab9990da4c854401e470b8d180/files/eclipse`
4. Download the Lombok from official site
`https://projectlombok.org/download`
5. Go to download folder and terminal from there.
![image](https://github.com/user-attachments/assets/fe4ed1a5-7a69-4a7e-b5c6-2e09051fe746)
6. type this command without new line
`**sudo**` is required becuase directly we can't paste the file there due to permissions.
`$sudo cp lombok.jar var/lib/flatpak/app/org.eclipse.Java/x86_64/stable/78f0828e03014f9b070ccefff48c738f5aac15ab9990da4c854401e470b8d180/files/eclipse`
7. Now go to path as per point no. 3
Type this command. Lombok UI will open paste the path there. and click install.
`$sudo java -jar lombok.jar`
8. It will open in taskbar, so pin that for every time!
![image](https://github.com/user-attachments/assets/1681d0ab-d0e4-4903-a441-3722b8bc82bb)
9. Now we can test in IDE.
![image](https://github.com/user-attachments/assets/57d9e311-87f0-4b30-8e1d-f4507c27d00d)

10. Booooooooooom! It's working!
