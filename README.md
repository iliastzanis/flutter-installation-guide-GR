# Εγκατάσταση Flutter στον υπολογιστή **(Windows)**.

## Εγκατάσταση του Flutter SDK:

1. Αρχικά κατεβάζουμε και κάνουμε εγκατάσταση το Git από [εδώ](https://git-scm.com/download/win).

2. Ύστερα κατεβάζουμε το [Flutter SDK](https://docs.flutter.dev/get-started/install/windows).

>### **ΠΡΟΣΟΧΗ!**
> - Μόλις κατεβάσουμε το SDK θα δούμε ένα αρχείο μορφής **.zip** το οποίο πρέπει να το κάνουμε **εξαγωγή** στον δίσκο που βρίσκονται και τα **Windows**. Για παράδειγμα: `C:\Users\yourName\Documents\Flutter`
> - **Δεν** πρέπει να κάνουμε εξαγωγή το αρχείο σε φάκελο όπως ο `Programm Files` καθώς χρειάζεται δικαιώματα διαχειριστή.
> - Ο φάκελος που θα το κάνουμε εξαγωγή **δεν** πρέπει να περιέχει κενά και ειδικούς χαρακτήρες.

## Εισαγωγή εντολών Flutter στο Terminal

Για να μπορέσουμε να χρησιμοποιήσουμε τις εντολές Flutter από το τερματικό θα πρέπει να επεξεργαστούμε το path.

1. Στην αναζήτηση των Windows ψάχνουμε `env` και επιλέγουμε `Edit the system environment variables`.

2. Από εκεί επιλέγουμε `Environment Variables`.

3. Στο `User variables` επιλέγουμε το `path` και το κάνουμε `Edit`.

4. Ύστερα επιλέγουμε `New` και βάζουμε την τοποθεσία που κάναμε εξαγωγή το Flutter SDK πχ: `C:\Users\yourName\Documents\Flutter`

> Εάν δεν υπάρχει to `path`, το δημιουργούμε επιλέγοντας `new` και για `Variable name` βάζουμε `path` και στο `Variable value` βάζουμε την τοποθεσία που κάναμε εξαγωγή το Flutter SDK πχ: `C:\Users\yourName\Documents\Flutter`

5. Για να βεβαιωθούμε ότι το κάναμε σωστα, ανοίγουμε ένα τερματικό οπουδήποτε και εκτελούμε την εντολή `flutter doctor`

Θα πρέπει να λάβουμε μία έξοδο της μορφής: 
```
[-] Android toolchain - develop for Android devices
    • Android SDK at D:\Android\sdk
    ✗ Android SDK is missing command line tools; download from https://goo.gl/XxQghQ
    • Try re-installing or updating your Android SDK,
      visit https://docs.flutter.dev/setup/#android-setup for detailed instructions.
```
> Ολά τα errors θα τα διωρθόσουμε σε επόμενα βήματα, σημασία έχει το τερματικό μας να μπορεί να εκτελεί εντολές που ξεκινάνε με τη λέξη flutter.

## Εγκατάσταση Android Studio (**Απαραίτητο**)

1. Κατεβάζουμε το [Android Studio](https://developer.android.com/studio).

2. Κάνουμε εγκατάσταση το `.exe` αρχείο. Αυτό εγκαθιστά τις τελευταίες εκδόσεις των Android SDK, Android SDK Command-line Tools, και Android SDK Build-Tools τα οποία είναι **απαραίτητα** για να μπορέσουμε να χρησιμοποιήσουμε το Flutter.

3. Μόλις τελειώσει η εγκατάσταση του Android Studio πηγάινουμε στο τερματικό και ξανατρέχουμε την εντολή `flutter doctor` για να βεβαιωθούμε ότι το Flutter έχει εντοπίσει το Android Studio.

4. Ανοίγουμε το Android Studio και επιλέγουμε τις **τρεις κουκίδες** (Πάνω δεξιά).

5. Επιλέγουμε `SDK Manager` και στο tab `SDK Platforms` επιλέγουμε την τελευταία έκδοση `Android` (Android 13 Tiramisu) και κάνουμε εγκατάσταση.

6. Αφού ολοκληρωθεί επιλέγουμε το tab `SDK Tools` και ελέγχουμε εάν είναι εγκατεστημένα τα παρακάτω tools:
> - Android SDK Build Tools
> - Android SDK Command Line Tools (latest)
> - Android Emulator
> - Android SDK Platform Tools
> - Google Usb Driver
> - Intel x86 Emulator Accelerator (Haxm Installer)

Σε περίπτωση που δεν είναι, τα κάνουμε εγκατάσταση.

7. Στην αρχική σελίδα του Android Studio στο αριστερό tab επιλέγουμε τα plugins, αναζητούμε και κάνουμε εγκατασταση τα παρακάτω:
> - Flutter
> - Dart

## Εγκατάσταση Visual Studio Code 
Γενικά μπορούμε να χρησιμοποιήσουμε το Android Studio για ανάπτυξη εφαρμογών με Flutter, ωστόσο είναι προτιμότερο το Visual Studio Code καθώς είναι ένας πιο ελαφρύς Editor και μαζί με κάποια Extensions επιταχύνει την ανάπτυξη εφαρμογών.

1. Κατεβάζουμε το [Visual Studio Code](https://code.visualstudio.com/) για Windows.

2. Κάνουμε εγκατάσταση το `.exe` στον υπολογιστή μας.

3. Επιλέγουμε στο αριστερό tab τα Extensions.

4. Κάνουμε αναζήτηση και εγκατάσταση των παρακάτω extensions:

>- Flutter
>- Dart

***Προαιρετικά*** μπορούμε να εγκαταστήσουμε και τα παρακάτω ώστε ο editor να γίνει πιο αποδοτικός, εύχρηστος και ευανάγνωστος:

>- Awesome Flutter Snippets
>- Bracket Pair Color DLW
>- Prettier - Code formatter
>- WSL

>### **ΠΡΟΣΟΧΗ!**
> To Visual Studio Code είναι διαφορετικό από το Visual Studio που αναφέρεται παρακάτω.


## Αποδοχή Android Licences

1. Ανοίγουμε τερματικό και πληκτρολογούμε `flutter doctor --android-licenses`

2. θα εμφανιστούν κάποιες άδειες χρήσης στις οποίες πρέπει να πατήσουμε `y` ώστε να τις αποδεχτούμε.

3. Στο τερματικό πληκτρολογούμε ξανά `flutter doctor` και θα πρέπει να μας εμφανιστεί η ακόλουθη έξοδος
```
Doctor summary (to see all details, run flutter doctor -v):
[✓] Flutter (Channel stable, 3.7.6, on Microsoft Windows [Version 10.0.22621.1413], locale en-US)
[✓] Windows Version (Installed version of Windows is version 10 or higher)
[✓] Android toolchain - develop for Android devices (Android SDK version 33.0.2)
[✓] Chrome - develop for the web
[✗] Visual Studio - develop for Windows
    ✗ Visual Studio not installed; this is necessary for Windows development.
      Download at https://visualstudio.microsoft.com/downloads/.
      Please install the "Desktop development with C++" workload, including all of its default components
[✓] Android Studio (version 2022.1)
[✓] VS Code (version 1.76.2)
[✓] Connected device (3 available)
[✓] HTTP Host Availability
```

Η παραπάνω έξοδος σημαίνει ότι είμαστε έτοιμοι να ξεκινήσουμε την ανάπτυξη εφαρμογών με τo Flutter.

>### **ΠΡΟΣΟΧΗ!**
>Στην δική μου εγκατάσταση δεν έχω το Visual Studio το οποίο είναι απαραίτητο **μόνο** εάν θέλουμε να αναπτύξουμε εφαρμογές για τα Windows. Όπως αναφέρθηκε και παραπάνω είναι διαφορετικό από το Visual Studio Code.

## Δημιουργία 1ης εφαρμογής με τη χρήση Flutter

1. Πηγαίνουμε σε έναν φάκελο στο υπολογιστή μας στον οποίο θέλουμε να έχουμε το Flutter Project μας.

2. Ανοίγουμε τερματικό μέσα στον φάκελο με τη χρήση `shift + δεξί κλικ -> New Terminal ή New Powershell Window`.

3. Πληκτρολογούμε την εντολή `flutter create project_name`. Το `project_name` μπορεί να είναι οποιοδήποτε όνομα στα αγγλικά χωρίς κενά και αποφεύγουμε τη χρήση ειδικών χαρακτήρων.

4. Μόλις ολοκληρωθεί η διαδικασία μπορούμε να κλείσουμε το τερματικό και να ανοίξουμε το Visual Studio Code.

5. Επιλέγουμε πάνω αριστερά το `File` και μετά `Open Folder`, εναλλακτικά χρησιμοποιούμε από το πληκτρολόγιο: `CTRL + K + O`.

6. Επιλέγουμε τον φάκελο που δημιουργήσαμε το Flutter Project μας.

7. Μόλις ανοίξει θα δούμε στο αριστερό pannel όλους τους φακέλους που περιέχει το project μας. Ένας από αυτούς τους φακέλους ονομάζεται `lib` και μέσα σε αυτόν βίσκεται το αρχείο `main.dart` το οποίο περιέχει τον κώδικα για το app μας.

## Τρέξιμο και αποσφαλμάτωση της εφαρμογής στο κινητό μας (**Visual Studio Code και μόνο για συσκευές Android**)

1. Ενεργοποιούμε από το Developer Options του κινητού μας το `Usb Debugging`.
> ### **Σημείωση 1:**
> Ο κάθε κατασκευαστής έχει διαφορετικό τρόπο οπότε πηγαίνουμε στον Browser μας και αναζητούμε: `How to enable Developer Options on (κατασκευαστής και μοντέλο της Android συσκευής μας)`.

> ### **Σημείωση 2:**
> Σε συσκευές `Xiaomi` πρέπει εκτός από το `Usb Debugging` να ενεργοποιήσουμε και δύο ακόμη ρυθμίσεις: `Install via Usb` και `Usb Debugging Security`. Περισσότερες πληροφορίες [εδώ](https://i.stack.imgur.com/wAjd5.jpg).

2. Συνδέουμε το κινητό μας στον υπολογιστή και επιλέγουμε `Trust this Computer` και στο κινητό μας θα υπάρχει η ειδοποίηση πως το `Usb Debugging` είναι ενεργοποιημένο.

3. Ανοίγουμε το Visual Studio Code και επιλέγουμε το project που δημιουργήσαμε στα προηγούμενα βήματα.

4. Επιλέγουμε το αρχείο `main.dart` με διπλό κλικ ώστε να το ανοίξει ο editor μας.

5. Κάτω δεξιά στη μπλε γραμμή θα πρέπει να βλέπουμε το μοντέλο του κινητού μας. Σε περίπτωση που βλέπουμε τη λέξη `Windows` πατάμε και επιλέγουμε τη συσκευή μας.

6. Πάνω δεξιά βρίσκεται η επιλογή να "τρέξουμε" τον κώδικα (Κουμπί Play). Ωστόσο εμείς θέλουμε να κάνουμε τρέξιμο και αποσφαλμάτωση οπότε θα επιλέξουμε το κάτω βελάκι και θα εμφανιστεί η επιλογή `Run and Debug` (Κουμπί Play μαζί με σκαθαράκι).

7. Η μπλε γραμμή θα γίνει πορτοκαλί και ανάλογα τη δύναμη του υπολογιστή μας θα γίνει εγκατάσταση της εφαρμογής στο κινητό μας σε περιόδο 3-8 λεπτά.

8. Μπορούμε πλέον να επεξεργαστούμε τον κώδικα του αρχείου `main.dart` και κάνοντας `save (CTRL + S)` κάθε φορά τις αλλαγές μας μπορούμε να τις βλέπουμε απευθείας στο κινητό μας!

<br>

> ### **Ηλίας Τζάνης** 
> #### *MSc in Big Data Driven Networked Systems | BSc in Computer Science | Software Developer*
