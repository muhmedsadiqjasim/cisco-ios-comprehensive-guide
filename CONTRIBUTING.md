# Contributing to the Cisco IOS Comprehensive Guide

First off, thank you for considering contributing to the **Cisco IOS Comprehensive Guide**! This project is community-driven, and we rely on network engineers and students like you to make this the best, most practical Cisco IOS reference on the internet.

Please read through these guidelines to ensure your contributions match the project standards and can be reviewed and merged quickly.

---

## 1. Claiming a Topic (Start Here)
To prevent duplicate work, **you must claim a topic before you start writing.**

1. Check the **Issues** tab to see if someone else is already working on the topic you want.
2. If it is open, create a new Issue stating: *"I would like to work on [Topic Name]"*.
3. Wait for a maintainer to assign the issue to you. Once assigned, it's all yours!

## 2. Branch Naming Strategy
When you are ready to start working, fork the repository and create a new branch. Please use the following naming conventions:
* For new topics: `feature/topic-name` (e.g., `feature/ospf-multi-area`)
* For corrections/updates: `fix/topic-name` (e.g., `fix/vlan-typo`)

## 3. Lab Files & Topology Rules (Crucial)
A major goal of this project is allowing learners to practice immediately. If you are submitting a new topic, you **must** include the lab file and a topology image.

### Lab File "Starting State" Rule
The lab file you provide must be at the **starting state before the configuration for that specific topic is applied**.
* **Basic Topics:** If the topic is "Passwords," the devices in the lab file should be completely blank. The learner will follow your markdown guide to add the passwords.
* **Advanced Topics:** If the topic is "Dynamic NAT," the lab file should have all baseline configurations already applied (Hostnames, IP addresses, basic routing) so the learner doesn't waste time setting up the basics. However, the **NAT configuration must be left completely empty**. The markdown guide will provide the NAT solution.

### Topology Images
* Take a **clear screenshot** of the topology directly from the lab application you are using.
* Ensure device hostnames and interface labels (e.g., `Gi0/1`) are clearly visible in the screenshot and match your configuration code.

## 4. Documentation Standards
Every topic must look and feel the same. 

1. **Use the Template:** Copy the `_template.md` file from the root directory, rename it to `README.md`, and place it in your topic's folder.
2. **Folder Structure:** Place your `README.md`, your topology image, and your lab file inside a **single, dedicated folder** for that topic. (Do not put lab files or images in the main root folder).
3. **App Declaration:** In your Pull Request and within the Requirements section of your `README.md`, clearly state the app name you used to build the lab (e.g., *Packet Tracer*, *EVE-NG*, *GNS3*).

## 5. Submitting a Pull Request
When you are ready to submit:
1. Ensure your markdown is clean and renders correctly.
2. Ensure you have included the lab file and the topology screenshot in the topic folder.
3. Open a Pull Request and fill out the template. Include the phrase `Closes #[Issue Number]` so GitHub automatically links your PR to your original claim issue.

## 6. Questions and Discussions
If you are stuck, need clarification on a topic, or want to discuss a new idea, please use the **GitHub Discussions** tab. We are happy to help you get your contribution over the finish line!

Once again, thank you for helping us build the ultimate networking cookbook!
