# MY TO-DO LIST APP

Το "My To-Do List" είναι μία βοηθητική εφαρμογή διαχείρισης εργασιών και υποχρεώσεων. Απευθύνεται σε μικρούς και μεγάλους που επιθυμούν να οργανώσουν και να προγραμματίσουν την καθημερινότητά τους, αφού μέσω αυτής ο καθένας μπορεί να προσθέσει και να παρακολουθήσει τις καθημερινές του εργασίες.

## Table of Contents
- [Οδηγίες Εγκατάστασης](#οδηγίες-εγκατάστασης)
- [Οδηγίες Χρήσης](#οδηγίες-χρήσης)
- [Δομή Εφαρμογής](#δομή-εφαρμογής)


## Οδηγίες Εγκατάστασης 
Για την εγκατάσταση της εφαρμογής ακολουθήστε τα παρακάτω βήματα:

**Βήμα 1:** Λήψη του συμπιεσμένου αρχείου της εφαρμογής σε έναν τοπικό φάκελο του υπολογιστή και αποσυμπίεση.

**Βήμα 2:** Εγκατάσταση της Python ή έλεγχος πληκτρολογώντας:

    python --version
    
**Βήμα 3:** Δημιουργία Εικονικού Περιβάλλοντος:

    python -m venv venv

**Βήμα 4:** Ενεργοποίηση Εικονικού Περιβάλλοντος:

  - Για να ενεργοποιήσετε το εικονικό περιβάλλον, χρησιμοποιήστε τις παρακάτω εντολές:
    - Σε Windows:
              
          .\venv\Scripts\activate
    - Σε macOS/Linux:
          
          source venv/bin/activate
    
**Βήμα 5:** Εγκατάσταση της Flask:

      pip install flask

**Βήμα 6:** Εκκίνηση της εφαρμογής:
  - Ανοίξτε το αρχείο app.py. Επιλέξτε "Run Python File". Πατήστε "Ctrl" και "click"   στον σύνδεσμο της μορφής: http://127.0.0.1:5000/ , που θα εμφανιστεί στο terminal.

#
Με αυτά τα βήματα θα μπορείτε πλέον να χρησιμοποιήσετε την εφαρμογή.
#


## Οδηγίες Χρήσης
Η εφαρμογή αποτελείται από τρεις σελίδες:
- Αρχική/Home
- Η Λίστα μου/My List
- Ρυθμίσεις/Settings

Ανοίγοντας την εφαρμογή θα βρεθείτε στην Αρχική σελίδα.
- **Προσθήκη εργασίας:** Για να προσθέσετε μια εργασία, θα πληκτρολογήσετε τον τίτλο της στο κενό με όνομα "Τίτλος" και την προθεσμία της στα κενά με ονόματα "Ημ/νία" και "Ώρα". Η προσθήκη ώρας δεν είναι απαραίτητη και μπορείτε να την παραλείψετε. Αφού συμπληρώσετε τα κενά, πατήστε το κουμπί "Προσθήκη" για να προστεθεί η εργασία σας στη λίστα. Πατώντας το κουμπί θα μεταφερθείτε στην σελίδα "Η Λίστα μου" στην οποία θα μπορείτε να δείτε όλες τις καταχωρημένες εργασίες.
- **Διαγραφή εργασίας:** Για να διαγράψετε/αφαιρέσετε μια εργασία από την λίστα σας πατήστε το κουμπί με το σύμβολο "x" στα αριστερά της εργασίας.
- **Άλλες λειτουργίες:** Στην σελίδα "Η Λίστα μου" μπορείτε να επισημάνετε μια εργασία ως "ολοκληρωμένη" πατώντας το λευκό κουτάκι (κάνοντας check). Επίσης, πατώντας το κουμπί "+Πρόσθεσε εργασία", θα μεταφερθείτε στην αρχική σελίδα για να προσθέσετε την επόμενη εργασία σας. Στην Αρχική σελίδα, θα δείτε δύο πλαίσια με τίτλους "Σήμερα" και "Αυτή την εβδομάδα". Στα πλαίσια αυτά θα εμφανίζονται αντίστοιχα οι εργασίες με προθεσμία την "σημερινή" ημερομηνία και τις ημερομηνίες όλης της εβδομάδας. Τέλος, σε όλες τις σελίδες υπάρχει η επιλογή γλώσσας δίπλα από το μενού με το οποίο αλλάζετε τις σελίδες.
- **Επιλογή χρωματικού θέματος:** Για να επιλέξετε χρωματικό θέμα, μεταβείτε στην σελίδα "Ρυθμίσεις" και πατήστε το επιθυμητό χρώμα (μωβ-προεπιλογή, μπλε, ροζ, πορτοκαλί, πράσινο, σκούρο).


## Δομή Εφαρμογής

- `app.py`: Το κύριο αρχείο της εφαρμογής.
- `templates/`: Ο φάκελος με τα τρία αρχεία HTML της εφαρμογής:
  - `home.html`: Ο κώδικας για την Αρχική σελίδα.
  - `my_list.html`: Ο κώδικας για την σελίδα "Η Λίστα μου".
  - `settings.html`: Ο κώδικας για την σελίδα "Ρυθμίσεις".
- `static/css/`: Ο φάκελος που περιέχει τον κώδικα σε CSS και τα εικονίδια της εφαρμογής.
  - `main1.css`: Ο κώδικας CSS για το styling της εφαρμογής.
- `tasks.txt`: Το αρχείο στο οποίο καταγράφονται οι εργασίες. Θα δημιουργηθεί αυτόματα αν δεν υπάρχει.
