# 🧪 Aether

<p>This repository was created to hold the configuration and documentation sourrounding my homelab. I hope you enjoy learning about it as much as I enjoyed building it!</p>
<p>Aether is the name of my homelab, inspired by the Greek god Aether, the god of light and the sky. The "light" represents the speed of network communication, which in fiber cables travels at about two-thirds the speed of light. The "sky" symbolizes cloud computing—in this case, my own personal cloud at home.</p>
<p>I built this homelab to serve as a space for experimentation, learning, and building clusters. It provides me with an environment where I can test out new or unfamiliar technologies, re-create/troubleshoot issues, and refine my skills without impacting a production environment.</p>

<h1>⚙️ Hardware</h1>
<p>Lenovo Legion Y530:</p>
<p>- i5-8300H CPU</p>
<p>- 16GB RAM (DDR4)</p>
<p>- 500GB SSD</p>

<h1>📐 Node Setup</h1>
<p>With the limited resources available (16GB RAM), I decided to go with the following split:</p>

| Node Type     | CPU | RAM |
| ------------- |---- | ----|
| Control Plane | 1   | 2GB |
| Worker Node 1 | 2   | 4GB |
| Worker Node 2 | 2   | 4GB |

<p>This should balance both memory and CPU allocation without overcommiting any hardware</p>

<h1>🛠️ Cluster Provisioning</h1>
<p>I decided to use Proxmox & K3s (https://k3s.io/) for the Kubernetes cluster on this home lab setup. K3s is a lightweight Kubernetes distribution that is specifically designed for resource-constrained environments, making it a perfect match for my hardware limitations.</p> 
<p> K3s allows me to scale down or tear down the cluster when not in use, preserving my laptop's performance and longevity. This aligns perfectly with the purpose of this cluster—not to host large applications or to run multiple databases, but to serve as a flexible playground environment. It’s a setup that I can break, tear down, and spin back up quickly, enabling me to learn, test, and iterate efficiently without any overhead or complexity.</p>
