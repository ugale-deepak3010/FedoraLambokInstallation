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
