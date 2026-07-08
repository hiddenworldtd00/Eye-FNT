# EYE_FNT - Système de Surveillance & Analyse Environnementale
<img width="1184" height="864" alt="result (6)" src="https://github.com/user-attachments/assets/6d63dc39-eb60-4cf9-89c7-e5e23c2e4a20" />


**Développé par les Hackers Tchadiens - HiddenWorld Community**

```
        ████████
      ██░░░░░░░░██
    ██░░░░░░░░░░░░██
   ██░░░░▓▓▓▓░░░░░░██
  ██░░░░▓▓██▓▓▓▓░░░░░██
  ██░░░░▓▓████▓▓▓░░░░██
   ██░░░░▓▓▓▓▓▓░░░░██
    ██░░░░░░░░░░░░██
      ██░░░░░░░░██
        ████████
        E Y E _ F N T
```

EYE_FNT est un système avancé de surveillance et d'analyse environnementale développé pour Linux. Il combine la vision par ordinateur (MediaPipe), l'analyse des réseaux sans fil (WiFi, Bluetooth), la détection des champs électromagnétiques, et bien plus encore dans une interface unifiée.

## ⚠️ Avertissement Légal

**Ce logiciel est STRICTEMENT réservé à un usage légal et éthique :**
- ✅ Surveillance de VOTRE propre propriété
- ✅ Tests de sécurité sur vos propres réseaux
- ✅ Recherche et développement en cybersécurité
- ✅ Éducation et formation

**INTERDICTIONS :**
- ❌ Espionner des personnes sans leur consentement
- ❌ Accéder à des réseaux sans autorisation
- ❌ Toute activité illégale ou malveillante

## 🎯 Fonctionnalités (40+)

### 1. MediaPipe & Vision (1-10)
- Détection faciale en temps réel
- Détection des mains et gestes
- Pose corporelle complète
- Segmentation selfie
- Suivi des iris
- Reconnaissance faciale avancée (Face Mesh)
- Détection d'objets
- Reconnaissance de gestes
- Analyse des expressions
- Suivi du regard

### 2. WiFi & Réseaux (11-20)
- Scan des réseaux WiFi
- Analyse du signal en temps réel
- Détection d'intrusion (Deauth)
- Capture de handshake WPA
- Test WPS
- Evil Twin (éducatif)
- Déauthentification (éducatif)
- Analyse du trafic
- Cartographie des réseaux
- Audit de sécurité WiFi

### 3. Bluetooth & RF (21-25)
- Scan des appareils Bluetooth
- Sniffing Bluetooth
- Détection de beacons
- Analyse des protocoles RF
- Brouillage de signaux (éducatif)

### 4. Électromagnétique (26-30)
- Scan des fréquences
- Analyse du spectre
- Détection des ondes ELF
- Mesure du champ magnétique
- Cartographie EMF de la pièce

### 5. Audio & Micro (31-35)
- Écoute du micro en temps réel
- Analyse spectrale audio
- Détection de fréquences
- Enregistrement audio
- Analyse des ultrasons

### 6. Système & Monitoring (36-40)
- Monitoring CPU/GPU/RAM
- Température système
- Processus actifs
- Connexions réseau
- Logs système en temps réel

### 7. Outils Avancés (41-45)
- Port scanning
- Banner grabbing
- WHOIS lookup
- DNS enumeration
- Génération de rapports

## 📋 Prérequis

- **OS** : Linux (Kali Linux, Ubuntu, Parrot OS recommandés)
- **Python** : 3.8 ou supérieur
- **Hardware** : Caméra, carte WiFi compatible monitor mode, adaptateur Bluetooth
- **Droits** : Root pour certaines fonctionnalités

## 🚀 Installation

### 1. Cloner le repository
```bash
git clone https://github.com/hiddenworld/EYE_FNT.git
cd EYE_FNT
```

### 2. Installer les dépendances système
```bash
sudo apt update
sudo apt install -y python3-pip python3-dev libffi-dev libssl-dev \
    libxml2-dev libxslt1-dev zlib1g-dev libjpeg-dev libpcap-dev \
    aircrack-ng wireshark tshark iw hcitool bluez libbluetooth-dev
```

### 3. Installer les dépendances Python
```bash
pip3 install -r requirements_EYE_FNT.txt
```

### 4. Configurer les permissions
```bash
sudo usermod -aG wireshark $USER
sudo setcap cap_net_raw,cap_net_admin=eip $(which python3)
```

## 🎮 Utilisation

### Lancer l'application
```bash
sudo python3 EYE_FNT.py
```

### Menu Principal
```
╔══════════════════════════════════════════════════════════════╗
║                    E Y E _ F N T                             ║
║         Système de Surveillance & Analyse                    ║
║              HiddenWorld - Hackers Tchadiens                 ║
╠══════════════════════════════════════════════════════════════╣
║                                                              ║
║  [1]  MediaPipe - Détection Visage                          ║
║  [2]  MediaPipe - Détection Mains                           ║
║  [3]  MediaPipe - Pose Corporelle                           ║
║  [4]  MediaPipe - Segmentation Selfie                       ║
║  [5]  MediaPipe - Suivi Iris                                ║
║  [6]  MediaPipe - Face Mesh                                 ║
║  [7]  MediaPipe - Détection Objets                          ║
║  [8]  MediaPipe - Reconnaissance Gestes                     ║
║  [9]  MediaPipe - Expressions Faciales                      ║
║  [10] MediaPipe - Suivi Regard                              ║
║                                                              ║
║  [11] WiFi - Scan Réseaux                                   ║
║  [12] WiFi - Analyse Signal                                 ║
║  [13] WiFi - Détection Intrusion                            ║
║  [14] WiFi - Capture Handshake                              ║
║  [15] WiFi - Test WPS                                       ║
║  [16] WiFi - Evil Twin (Éducatif)                           ║
║  [17] WiFi - Déauthentification (Éducatif)                  ║
║  [18] WiFi - Analyse Trafic                                 ║
║  [19] WiFi - Cartographie Réseaux                           ║
║  [20] WiFi - Audit Sécurité                                 ║
║                                                              ║
║  [21] Bluetooth - Scan Appareils                            ║
║  [22] Bluetooth - Sniffing                                  ║
║  [23] Bluetooth - Beacons                                   ║
║  [24] RF - Analyse Protocoles                               ║
║  [25] RF - Brouillage (Éducatif)                            ║
║                                                              ║
║  [26] EM - Scan Fréquences                                  ║
║  [27] EM - Analyse Spectre                                  ║
║  [28] EM - Détection Ondes ELF                              ║
║  [29] EM - Champ Magnétique                                 ║
║  [30] EM - Cartographie Pièce                               ║
║                                                              ║
║  [31] Audio - Écoute Micro                                  ║
║  [32] Audio - Analyse Spectrale                             ║
║  [33] Audio - Détection Fréquences                          ║
║  [34] Audio - Enregistrement                                ║
║  [35] Audio - Analyse Ultrasons                             ║
║                                                              ║
║  [36] Système - Monitoring CPU/GPU/RAM                      ║
║  [37] Système - Température                                 ║
║  [38] Système - Processus                                   ║
║  [39] Système - Connexions Réseau                           ║
║  [40] Système - Logs Temps Réel                             ║
║                                                              ║
║  [41] Outils - Port Scanning                                ║
║  [42] Outils - Banner Grabbing                              ║
║  [43] Outils - WHOIS Lookup                                 ║
║  [44] Outils - DNS Enumeration                              ║
║  [45] Outils - Génération Rapport                           ║
║                                                              ║
║  [99] Mode Surveillance Continue                            ║
║  [0]  Quitter                                               ║
╚══════════════════════════════════════════════════════════════╝
```

## 📊 Exemples d'utilisation

### Détection Faciale
```
[+] Lancement MediaPipe - Détection Visage...
[*] Appuyez sur 'q' pour quitter
[*] Visages détectés: 2
    - Visage #1: Confiance 95% | Position: (120, 80)
    - Visage #2: Confiance 87% | Position: (400, 150)
```

### Scan WiFi
```
[+] Scan des réseaux WiFi...
[*] 5 réseaux trouvés:
  [1] MonReseau5G
      Signal: -45 dBm
      Canal: 36 | Sécurisé
  [2] Free_WiFi
      Signal: -67 dBm
      Canal: 6 | OUVERT ⚠️
```

### Analyse Électromagnétique
```
[+] Analyse du spectre électromagnétique...
[*] Fréquences détectées:
    - 2.412 GHz: WiFi Canal 1 | Intensité: -42 dBm
    - 2.437 GHz: WiFi Canal 6 | Intensité: -38 dBm
    - 2.480 GHz: Bluetooth | Intensité: -55 dBm
```

## 🔧 Configuration

Le fichier de configuration `config.json` permet de personnaliser :
- Interface WiFi par défaut
- Seuils de détection
- Dossier de sauvegarde
- Options d'affichage

## 📝 Logs

Toutes les activités sont loguées dans `eye_fnt_log_YYYYMMDD_HHMMSS.json` :
```json
{
  "timestamp": "2024-01-15T14:30:00",
  "action": "wifi_scan",
  "details": "15 réseaux trouvés",
  "user": "root"
}
```

## 🤝 Contribution

**HiddenWorld Communauté Tchadienne**
- Discord : [Lien]
- Telegram : [Lien]
- GitHub : [Lien]

## 📜 Licence

MIT License - Usage éducatif et légal uniquement

---

**👁️ EYE_FNT - L'œil qui voit tout, dans le respect de la loi.**
