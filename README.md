1. Install lombok in eclipse using marketplace
![image](https://github.com/user-attachments/assets/51d12f07-f696-41e3-beb1-bb62fbeec035)

2. Refer this Screenshot and use this URL
`https://projectlombok.org/p2`
![image](https://github.com/user-attachments/assets/53be48a2-c340-417a-8134-f48854404e6f)


3. Add this highlighted text based on your system path in .desktop file:
here is the file location : `/var/lib/flatpak/exports/share/applications`

- [ ] Might be you have different username: `dipakugale`
- [ ] Might be you have different lombok version: `/org.projectlombok.agent_1.18.36/`
This is the code you have to update.
`-- -vmargs -javaagent:/home/dipakugale/.var/app/org.eclipse.Java/eclipse/plugins/org.projectlombok.agent_1.18.36/lombok.jar`

![image](https://github.com/user-attachments/assets/67ffd053-0b97-4ec9-bb73-8f61132db535)

4. Restart laptop & eclipse several times.

_____________________________________________________

### How to install maven in Fedora or Windows?

1. Download maven zip file from here
`https://maven.apache.org/download.cgi`
2. Extract zip file anywhere in file explorer
Example: `/home/dipakugale/Documents/ImpPath/InstalledSoftwareHereDoNotDelete/apache-maven-3.9.9`
3. Now paste the path here
![image](https://github.com/user-attachments/assets/ec306483-3bdd-4649-9173-d637da08d502)

4. Now maven should be work:
![image](https://github.com/user-attachments/assets/ab8722dc-8d73-4b96-9a3e-1a75a6ab2cee)

5. Expected result should be work.

![image](https://github.com/user-attachments/assets/7d7ec64a-3b3e-467a-aaa4-73a78bd4c28a)


