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
[https://projectlombok.org/download](url)
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

10. Booooooooooom! It's working
.
___________________________________________

### Now let talk to the desktop shortcut.

_Why it's very important....?_

1. I have installed eclipse using flatpak/ software store
2. Then I installed lombok in somewhere.
3. But...
4. Flatpak is encapsulated environment where we can't modify directly code.
5. Hence above steps can be work and can't!
6. We need to pass one parameter to the eclipse (Note: this is standard for Lombok for any IDE or any OS)
7. Here that parameter:

`
-- -vmargs -javaagent:/home/dipakugale/.var/app/org.eclipse.Java/eclipse/plugins/org.projectlombok.agent_1.18.34/  @@ %f @@
`

9. Now we have to pass this parameter when we open the desktop shortcut
10. But flatpak shortcuts are always present here:
`/var/lib/flatpak/exports/share/applications`
12. So this link is referred to this location
`/var/lib/flatpak/app/org.eclipse.Java/current/active/export/share/applications`
13. So we have to modify this file:
`org.eclipse.Java.desktop`
14. Now it should be look like this
`Exec=/usr/bin/flatpak run --branch=stable --arch=x86_64 --command=eclipse --file-forwarding org.eclipse.Java -- -vmargs -javaagent:/home/dipakugale/.var/app/org.eclipse.Java/eclipse/plugins/org.projectlombok.agent_1.18.34/  @@ %f @@`
15. Please note making any single change in `.desktop `file laptop need to restart then it will reflect.
16. Happy journey!
.
.
!

                                              *** THANK * YOU ***
