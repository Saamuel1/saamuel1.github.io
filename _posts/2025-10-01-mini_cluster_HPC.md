---
title: "Reproduction d'un mini cluster HPC"
date: 2025-10-01
categories: [Projets, IA, HPC, Kubernetes]
tags: [Python, Kubernetes, docker, contenerisation]
---

## Objectif
Reproduire à petite échelle ce que font les grands centres de calcul :  
→ faire tourner plusieurs machines virtuelles comme un **cluster** capable d’exécuter des conteneurs IA.

Ce projet montre ma capacité à :
- Installer et configurer **Kubernetes** manuellement (sans outils automatiques)
- Connecter plusieurs machines pour créer un **cluster distribué**
- Gérer du **stockage partagé**, comme dans un vrai environnement HPC
- Déployer des **pods** (applications conteneurisées) sur plusieurs nœuds

---

## Architecture du projet
- **1 master node** (coordonne les ressources)
- **2 worker nodes** (exécutent les pods)
- **Stockage NFS** partagé entre les trois
- **Réseau Flannel** pour la communication interne

L’ensemble tourne sur mon PC local grâce à **Multipass / VirtualBox**, avec **Ubuntu 22.04** sur chaque VM.

---

## Étapes principales
1. Création des 3 machines virtuelles  
2. Installation manuelle de Kubernetes (kubeadm, kubelet, containerd)  
3. Initialisation du cluster (`kubeadm init`)  
4. Connexion des workers (`kubeadm join`)  
5. Mise en place d’un **réseau de pods (Flannel)**  
6. Configuration d’un **stockage partagé NFS**  
7. Déploiement d’un **pod Nginx** pour test  

---

## Résultats obtenus
- ✅ 3 nœuds interconnectés (`Ready`)
- ✅ Stockage commun monté sur chaque machine
- ✅ Pod Nginx déployé et accessible
- ✅ Démonstration fonctionnelle d’un environnement IA–HPC miniature

---

## Compétences démontrées
- Kubernetes / Containerd / kubeadm
- Réseau et CNI (Flannel)
- Systèmes Linux (Ubuntu 22.04)
- NFS et stockage distribué
- Déploiement de pods / orchestration
- Diagnostic (swap, cgroups, IP forwarding, etc.)

---

## Perspectives
Ce mini-cluster servira de base à mes prochains projets :
- **Intégrer Slurm et Podman** pour exécuter des jobs IA
- **Containeriser des modèles IA** (PyTorch, TensorFlow)
- **Simuler un environnement HPC complet sur laptop**

---

🔗 [Lien GitHub du projet](https://github.com/Saamuel1/MiniCluster_Kubernetes/tree/main)
---

**Ce projet prouve que je sais construire un cluster Kubernetes from scratch, comprendre sa logique interne, et l’adapter à des besoins IA–HPC concrets.**
