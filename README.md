# Billz-Desktop-Updater
Releasing new versions for Billz desktop app

Steps for new release:
1. Upgrade verion number in msix file, version.txt and pubspec.yaml files on project
2. Upgrade version number on github pages (which application checks). It should the same as your project's verion.
3. Run this commands on app's path:
  - flutter build windows
  - flutter pub run msix:create  
  After successfully msix file generated create new release on GitHub or update old one.
\nVoila! It should check and update new version
