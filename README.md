---

# 🎮 Maher's Minecraft Server Guide

## 🚀 Create a Minecraft Server Using GitHub Codespaces (No Panel Required!)

Yes, you read that right — **no need for PufferPanel or Pterodactyl!** You can now create a fully working Minecraft server **directly from GitHub** using Codespaces.

---

## 📌 Steps to Get Started

### ✅ Step 1: Create a Repository

1. Go to [GitHub](https://github.com/) and click **New Repository**.
   
   ![Step One](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20One.png)
   
3. Name your repo anything you like, and choose either Public or Private.
   ✅ IMPORTANT: Check the box for “Add a README file”. This will automatically initialize the repo — you no longer need to create a file manually.
   
   ![Step Two](https://github.com/user-attachments/assets/50c439d1-05bd-4d2c-b2e8-055375d7a90b)
   
---

### ✅ Step 2: make a GitHub Codespace

1. Click the **Code** button, then go to **Codespaces** Click the **More** button and Click the **New with options"" button.

   ![Step Three](https://github.com/user-attachments/assets/16455a4a-1677-4799-8316-2ae4517ab73f)

2. Choose your "Region", Set **Machine type** too **4-Core** (16GB RAM - 32GB Storge) and Create your Codespace.
   
   ![Step Four](https://github.com/user-attachments/assets/e76b37d9-e76a-45f0-92c7-b2d272e35b6f)
   ![Step Five](https://github.com/user-attachments/assets/fa347c13-0286-4517-ab5e-c84760b56852)
   ![Step Six](https://github.com/user-attachments/assets/b78a954f-f114-4d3d-889d-91fe28c778d6)

---

### ✅ Step 3: Setup the Server in Codespace

1. First, update packages:

   ```bash
   sudo apt update && sudo apt upgrade
   ```

2. Go to the [PaperMC Downloads](https://papermc.io/downloads/paper) page.

   ![Step Seven](https://github.com/user-attachments/assets/e1f3083f-96e5-43b2-8e6e-9066dae50a18)

3. Right-click the latest `.jar` link, then copy the link.

4. In Codespace, download it using:

   ```bash
   wget (your-link-here)
   ```

   For example, for Minecraft 1.21.6:

   ```bash
   wget https://fill-data.papermc.io/v1/objects/c4bfc337e09100fdfd060a36b66174be87370d9975ace4e28e45d873ce992c62/paper-1.21.6-47.jar
   ```

5. Rename it to `paper.jar`:

   ```bash
   mv paper-*.jar paper.jar
   ```

6. Run the server:

   ```bash
   java -Xmx16G -Xms4G -jar paper.jar --nogui
   ```

7. When prompted, open `eula.txt`:

   ```bash
   nano eula.txt
   ```

   Change:

   ```txt
   eula=false
   ```

   to:

   ```txt
   eula=true
   ```

8. Save and re-run the server:

   ```bash
   java -Xmx16G -Xms4G -jar paper.jar --nogui
   ```

---

## 🎉 Success! Your Minecraft Server is Running!

You can now connect to your server (via the Codespace's exposed IP, or via tools like [ngrok](https://ngrok.com/) if needed).

You can also use Plugins like [Playit.gg](https://playit.gg/download/plugins) to connect to your server

---

## 🤝 Need Help?

Feel free to DM me on Discord: **qutomc**

Discord Server: [Maher's Den](https://discord.gg/tzn8JBenTc)

---
