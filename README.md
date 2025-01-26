# 🧪 Aether

<p>Aether is my homelab, the name is based on the greek god Aether, the god of light and the sky. Light relating to the speed at which networking communication (which is actaully 2/3rd's the speed of light) and the sky symoblising cloud computing, I guess in this instance my own personal cloud at home.</p>
<p>I built this homelab to serve as a space for experimentation, learning, and building systems. It provides an environment where I can test new or unfamiliar technologies, troubleshoot challenges, and refine my skills without impacting production environments.</p>

<h1>⚙️ Hardware</h1>
<p>Lenovo Legion Y530:</p>
<p>- i5-8300H CPU</p>
<p>- 16GB RAM (DDR4)</p>

<h1>📐 Architecture</h1>
<p>With the limited resources available (16GB RAM), I decided to go with the following setup:
| Node Type     | CPU | RAM |
| ------------- |---- | ----|
| Control Plane | 1   | 2GB |
| Worker Node 1 | 2   | 4GB |
| Worker Node 2 | 2   | 4GB |
</p>
<p>This should balance both memory and CPU allocation without overcommiting the hardware</p>

<h1>🛠️ Cluster Provisioning</h1>
<p>wip</p>
