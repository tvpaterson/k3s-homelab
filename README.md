# 🧪 Aether

<p>Aether is my homelab, the name is based on the greek god Aether, the god of light and the sky. Light relating to the speed at which networking communication (which is actaully 2/3rd's the speed of light) and the sky symoblising cloud computing, I guess in this instance my own personal cloud at home.</p>
<p>I built this homelab to serve as a space for experimentation, learning, and building systems. It provides an environment where I can test new or unfamiliar technologies, troubleshoot challenges, and refine my skills without impacting production environments.</p>

<h1>⚙️ Hardware</h1>
<p>Lenovo Legion Y530:</p>
<p>- i5-8300H CPU</p>
<p>- 16GB RAM (DDR4)</p>

<h1>📐 Node Setup</h1>
<p>With the limited resources available (16GB RAM), I decided to go with the following split:</p>

| Node Type     | CPU | RAM |
| ------------- |---- | ----|
| Control Plane | 1   | 2GB |
| Worker Node 1 | 2   | 4GB |
| Worker Node 2 | 2   | 4GB |

<p>This should balance both memory and CPU allocation without overcommiting the hardware</p>

<h1>🛠️ Cluster Provisioning</h1>
<p>I decided to use Proxmox & K3s (https://k3s.io/) for the Kubernetes cluster on this home lab setup. K3s is a lightweight Kubernetes distribution that is specifically designed for resource-constrained environments, making it a perfect match for my hardware limitations.</p> 
<p> K3s allows me to scale down or tear down the cluster when not in use, preserving my laptop's performance and longevity. This aligns perfectly with the purpose of this cluster—not to host large applications or to run multiple databases, but to serve as a flexible playground environment. It’s a setup that I can break, tear down, and spin back up quickly, enabling me to learn, test, and iterate efficiently without any overhead or complexity.</p>
