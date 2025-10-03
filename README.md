# 🛠️ workstation_automation

Automate the setup of your workstation for **DevOps / SRE / Platform Engineering** and more using **Ansible**.  
This project installs and configures essential packages, ensuring a fast and consistent setup across multiple operating systems.  

---

## 🚀 Features

- Automated installation of DevOps/SRE/Platform Engineering tools.
- Supports **Linux** and **macOS** (Intel and ARM).  
- Version management via `group_vars`.  
- Multi-role: easily enable or disable packages in `playbooks.yml`.  
- Packages without a defined version will always install the **latest available**.  

---

## 💻 Tested Systems

✅ Compatible and tested on the following operating systems:

- Ubuntu 22.04
- Ubuntu 24.04
- macOS Ventura 13.7.6 (Intel)
- macOS Sequoia 15.6.1 (ARM)
- macOS Tahoe 26.0 (ARM)

---

⚠️ Note: Docker installation may fail on newer versions of macOS. In such cases, you may need to perform a manual step to complete the setup.

---

## ⚙️ How to Use

### 1. Install Ansible
- [Official installation guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)  

### 2. Clone the repository
```bash
git clone https://github.com/leandrolanza/workstation_automation
cd workstation_automation
```

### 3. Run the playbook
```bash
ansible-playbook playbooks.yml --ask-become-pass
```

🔹 To disable the installation of a specific role, simply comment out the corresponding line in the playbooks.yml file.
```
  roles:
    - utilities
    - network_tools
    - docker
    - aws_tools
    - kubernetes_tools
    - hashicorp_tools
    - code_editor
    - spotify
```

---

## 📦 Installed Packages

### Cloud & CLI
- [AWS CLI](https://docs.aws.amazon.com/cli/)  
- [AWS VPN Client](https://aws.amazon.com/vpn/)  

### Dev Tools
- [Visual Studio Code](https://code.visualstudio.com/)  
- [Docker](https://www.docker.com/)  
- [Terraform](https://www.terraform.io/)  
- [Packer](https://www.packer.io/)  
- [Vault](https://www.vaultproject.io/)  

### Kubernetes
- [kubectl](https://kubernetes.io/docs/reference/kubectl/)  
- [kubens](https://github.com/ahmetb/kubectx)  
- [kubectx](https://github.com/ahmetb/kubectx)  
- [kube-score](https://kube-score.com/)  
- [kube-capacity](https://github.com/robscott/kube-capacity)  
- [kubent](https://github.com/doitintl/kube-no-trouble)  
- [k9s](https://k9scli.io/)  
- [Helm](https://helm.sh/)  
- [Lens](https://k8slens.dev/)  
- [stern](https://github.com/stern/stern)  

### Networking
- net-tools  
- whois  
- iputils-ping  
- dnsutils  
- traceroute  
- tcpdump  
- rdesktop  
- nmap  

### Productivity
- [Spotify](https://www.spotify.com/)  
- [Zsh](https://www.zsh.org/)  
- [Oh My Zsh](https://ohmyz.sh/)  
- [Postman](https://www.postman.com/)  
- [Google Chrome](https://www.google.com/chrome/)  
- [Slack](https://slack.com/)  

---

## 🤝 Contributing

Feel free to open issues and pull requests with improvements, new packages, or fixes.

---

## 📜 License

This project is licensed under the MIT License. You are free to use, modify, and distribute it under the terms of the license.