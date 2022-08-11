# Billz-Desktop/Mobile-Updater
Releasing new versions for [Billz desktop app]

Steps for new release:
1. Upgrade verion number in msix file, version.txt and pubspec.yaml files on project
2. Upgrade version number on github pages (which application checks). It should the same as your project's verion.
3. Run this commands on app's path:
  - flutter build windows
  - flutter pub run msix:create  
  After successfully msix file generated create new release on GitHub or update old one.

Voila! It should check and update new version

Releasing new versions for [Billz Mobile apps]

Steps for new release:
1. After all new changes push and merge it with dev stage(Change also version number in pubspec.yaml)
2. Get registered app bundle using Android studio and publish it in internal testing section
2. When Play Store review is finished, test last updates or give access to QA engineers to test
4. If everything is ok, then publish it to production there
5. Change release notes and version on github as well
That's it!
