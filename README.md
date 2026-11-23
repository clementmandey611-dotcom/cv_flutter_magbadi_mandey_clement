# Application Mobile CV - Magbadi Mandey Clement

<p align="center">
  <img src="pictures/profile.jpg" width="130" height="130" style="border-radius: 50%; object-fit: cover; border: 3px solid #1E3A8A;" alt="MAGBADI MANDEY CLEMENT" />
</p>

<p align="center">
  <b>MAGBADI MANDEY CLEMENT</b><br>
  <i>Étudiant en Licence Réseau Système et Télécommunication</i><br>
  Développeur Flutter • Web • Python
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.50.0-02569B?logo=flutter" alt="Flutter Badge" />
  <img src="https://img.shields.io/badge/Dart-3.14.0-0175C2?logo=dart" alt="Dart Badge" />
  <img src="https://img.shields.io/badge/Platform-Android%20%7C%20iOS%20%7C%20Web-success" alt="Platform" />
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License" />
</p>

---

## Démonstration Vidéo

**[Regarder la vidéo complète de la démo sur Google Drive](https://drive.google.com/file/d/1iHZg-fO8-dYtmE8TZ5euYogZEnTX7X3Z/view?usp=sharing)

## 📸 Aperçu de l'Application (Captures d'Écran)

<div align="center">

| Page de Connexion | Menu Latéral (Drawer) | Mon CV Complet |
| :---: | :---: | :---: |
| <img src="pictures/Screenshot_20261119-175331.png" width="220" alt="Connexion" /> | <img src="pictures/Screenshot_20261119-175409.png" width="220" alt="Drawer Latéral" /> | <img src="pictures/Screenshot_20261119-175345.png" width="220" alt="CV Accueil" /> |

| CV & Compétences | Cercle Familial | Mes Coordonnées |
| :---: | :---: | :---: |
| <img src="pictures/Screenshot_20261119-175352.png" width="220" alt="Compétences CV" /> | <img src="pictures/Screenshot_20261119-175400.png" width="220" alt="Famille" /> | <img src="pictures/Screenshot_20261119-175414.png" width="220" alt="Contacts" /> |

</div>

---

## 🎯 Description du Projet

Cette application mobile développée avec le framework **Flutter** met en valeur le parcours académique, les compétences techniques, la famille et les coordonnées directes de **MAGBADI MANDEY CLEMENT**.

Elle répond fidèlement aux exigences fonctionnelles et graphiques d'une application professionnelle moderne :

1. **Page de Connexion (`LoginScreen`)** :
   - Formulaire complet avec champ Identifiant et champ Mot de passe masqué (avec icône interactive pour masquer/afficher).
   - Validation dynamique des entrées.
   - Bouton stylé « Se connecter » avec animation de chargement.
   - Identifiants pré-remplis pour tester rapidement (`clement` / `123456`).

2. **Page d'Accueil - CV Complet (`CvScreen`)** :
   - **En-tête de Profil** : Photo réelle, nom complet, badge officiel `ETUDIANT`.
   - **Formation** : Licence en Réseau Système et Télécommunication.
   - **Expériences & Projets** :
     - Stage professionnel chez **Global Technology** (Réseau et Systèmes).
     - Projet : **Application de gestion d'une école** (solution logicielle complète).
   - **Compétences Techniques** : Developer Flutter, Développement Web, Python avec barres de progression.
   - **Compétences Linguistiques** : Français (Maîtrise), Lingala (Natif), English (Intermédiaire).
   - **Centres d'intérêt** : Football, le Réseau et Lire.

3. **Page Famille (`FamilyScreen`)** :
   - Présentation interactive des membres de la famille : nom, photo locale embarquée, lien de parenté, profession et description.
   - **Bascule d'affichage dynamique** : Possibilité d'alterner en un clic entre la vue **ListView** et la vue **GridView**.

<div align="center">

| Joseph Mandey (Père) | Marie Magbadi (Mère) | Patrick Mandey (Frère) |
| :---: | :---: | :---: |
| <img src="pictures/father.jpg" width="120" style="border-radius:50%" /> | <img src="pictures/mother.jpg" width="120" style="border-radius:50%" /> | <img src="pictures/brother.jpg" width="120" style="border-radius:50%" /> |
| **Ingénieur Télécom** | **Professeure & Entrepreneure** | **Admin Système & Cloud** |

| Grâce Mandey (Sœur) | David Magbadi (Cadet) |
| :---: | :---: |
| <img src="pictures/sister.jpg" width="120" style="border-radius:50%" /> | <img src="pictures/younger_brother.jpg" width="120" style="border-radius:50%" /> |
| **Étudiante en Médecine** | **Élève au Collège** |

</div>

4. **Page Contact (`ContactScreen`)** :
   - Coordonnées directes et cliquables grâce à `url_launcher` :
     - ✉️ **E-mail** : `clementmandey611@gmail.com` (ouvre le client de messagerie).
     - 📞 **Téléphone** : `0837378179` (lance le composeur téléphonique).
     - 💬 **WhatsApp Direct** : `0837378179` (ouvre une conversation WhatsApp instantanée).
     - 🐙 **GitHub** : Lien vers les dépôts et projets.
     - 💼 **LinkedIn** : Lien vers le profil professionnel.
   - Bouton de copie rapide dans le presse-papier pour chaque coordonnée.

5. **Navigation Ergonomique (`MainScreen`)** :
   - **NavigationBar** Material 3 en bas pour un passage fluide d'une page à l'autre.
   - **Drawer latéral** reprenant l'identité visuelle de l'utilisateur avec un bouton de **Déconnexion** sécurisé.

---

## 📁 Structure du Projet

```text
cv_flutter_magbadi_mandey_clement/
├── android/                   # Configuration native Android
├── assets/
│   └── images/
│       ├── profile.jpg        # Photo de profil réelle de Clément
│       └── family/            # Photos locales des membres de la famille
├── lib/
│   ├── main.dart              # Point d'entrée de l'application
│   ├── models/
│   │   └── family_member.dart # Modèle de données pour la famille
│   ├── screens/
│   │   ├── login_screen.dart   # Page 1 : Authentification
│   │   ├── main_screen.dart    # Conteneur de navigation (Bar + Drawer)
│   │   ├── cv_screen.dart      # Page 2 : CV Complet
│   │   ├── family_screen.dart  # Page 3 : Cercle familial (List/Grid)
│   │   └── contact_screen.dart # Page 4 : Coordonnées cliquables
│   └── theme/
│       └── app_theme.dart     # Charte graphique et thème Material 3
├── pictures/                  # Galerie d'images et captures d'écran pour GitHub
├── pubspec.yaml               # Dépendances (url_launcher, font_awesome_flutter)
└── README.md                  # Documentation du projet
```

---

## 🚀 Installation & Exécution

### Prérequis
- [Flutter SDK](https://docs.flutter.dev/get-started/install) (version 3.x ou supérieure)
- Android Studio ou VS Code avec les extensions Flutter/Dart
- Un appareil Android physique ou un émulateur connecté

### Commandes pour lancer l'application

1. Cloner le dépôt GitHub :
   ```bash
   git clone https://github.com/clementmandey/cv_flutter_magbadi_mandey_clement.git
   cd cv_flutter_magbadi_mandey_clement
   ```

2. Récupérer les dépendances :
   ```bash
   flutter pub get
   ```

3. Lancer l'application :
   ```bash
   flutter run
   ```

---

## 📬 Contact & Informations

- **Nom :** MAGBADI MANDEY CLEMENT
- **E-mail :** [clementmandey611@gmail.com](mailto:clementmandey611@gmail.com)
- **Téléphone / WhatsApp :** [+243 837 378 179](https://wa.me/243837378179)
- **Localisation :** Kinshasa, République Démocratique du Congo (RDC)
