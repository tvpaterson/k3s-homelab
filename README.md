# 🧪 Pi-nacle: Small Nodes, Big Ideas

<p>This repository was created to hold the configuration files and documentation sourrounding my homelab. I hope you enjoy learning about it as much as I enjoyed building it!</p>
<p>Pi-nacle is the name given to my homelab for the sole reason that it has reached it's pinnacle in terms of performance.</p>
<p>I built this homelab to serve as a space for experimentation, learning, and building clusters. It provides me with an environment where I can test out new or unfamiliar technologies, re-create/troubleshoot issues, and refine my skills without impacting any other environments.</p>

<h1>⚙️ Hardware</h1>
<p>Raspberry Pi 4b 8GB:</p>
<p>- x4 Raspberry Pi Zeros </p>
<p>Sporting a whopping 10GB of RAM, this little Pi of mine allows me to run a 6 node cluster that can fit in the palm of my hand. Using the Cluster Hat 2.5 I'm able to add 4 additional machines literally ontop of my Pi 4</p>

<h1>📐 Node Setup</h1>
<p>With the limited resources available (16GB RAM), I decided to go with the following split:</p>

| Node Type      | CPU | RAM  |
| -------------  |---- | -----|
| Control Plane  | 1   | 2GB  |
| x4 Worker Nodes| 1   | 512MB|


<p>This should balance both memory and CPU allocation without overcommiting any hardware</p>

<h1>🛠️ Cluster Provisioning</h1>
<p>I decided to use Proxmox & K3s (https://k3s.io/) for the Kubernetes cluster on this home lab setup. K3s is a lightweight Kubernetes distribution that is specifically designed for resource-constrained environments, making it a perfect match for my hardware limitations.</p> 
<p> K3s allows me to scale down or tear down the cluster when not in use, preserving my laptop's performance and longevity. This aligns perfectly with the purpose of this cluster—not to host large applications or to run multiple databases, but to serve as a flexible playground environment. It’s a setup that I can break, tear down, and spin back up quickly, enabling me to learn, test, and iterate efficiently without any overhead or complexity.</p>
