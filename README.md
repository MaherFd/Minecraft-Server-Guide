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
   
   ![Step Two](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20Two.png)
   
---

### ✅ Step 2: make a GitHub Codespace

1. Click the **Code** button, then go to **Codespaces** Click the **More** button and Click the **New with options"" button.

   ![Step Three](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20Three.png)

2. Choose your "Region", Set **Machine type** too **4-Core** (16GB RAM - 32GB Storge) and Create your Codespace.
   
   ![Step Four](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20Four.png)
   ![Step Five](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20Five.png)
   ![Step Six](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20Six.png)

---

### ✅ Step 3: Setup the Server in Codespace

1. First, update packages:

   ```bash
   sudo apt update && sudo apt upgrade
   ```

2. Go to the [PaperMC Downloads](https://papermc.io/downloads/paper) page.

   ![Step Seven](https://github.com/MaherFd/Minecraft-Server-Guide/blob/main/Step%20Seven.png)

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

You can now connect to your server by using Plugins like [Playit.gg](https://playit.gg/download/plugins) to connect to your server

You can also use via tools like [ngrok](https://ngrok.com/) , [cloudflare](https://dash.cloudflare.com/) (if needed).

---

## 🤝 Need Help?

Feel free to DM me on Discord: **qutomc**

Discord Server: [Maher's Den](https://discord.gg/tzn8JBenTc)

---
