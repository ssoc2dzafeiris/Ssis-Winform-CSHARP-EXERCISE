Σκοπός
Ο σκοπός της άσκησης είναι:
Α) Να κατασκευαστεί ένα SSIS Package που θα διαβάζει τα 5 txt αρχεία που σας δίνονται και θα τα αποθηκεύει σε αντίστοιχους πίνακες σε βάση δεδομένων Microsoft Sql Server.
B) Να κατασκευαστεί εφαρμογή σε C# .NET Windows Forms, η οποία 
    • θα κάνει unzip το password-protected archive (αρχείο Files.zip) με τα 5 αρχεία που σας δίνονται χρησιμοποιώντας εξωτερική library
    • θα καλεί το SSIS package που δημιουργήσατε στο βήμα A
    • θα περιέχει combo box όπου επιλέγοντας τον εκάστοτε οφειλέτη (Persons) θα εμφανίζεται η καρτέλα του με πληροφορίες για τον οφειλέτη
Πληροφορίες:
    • Η διαδικασία του unzip πρέπει να γίνει υποχρεωτικά χρησιμοποιώντας εξωτερική βιβλιοθήκη και όχι κάποιο .NET feature. Για τη διευκόλυνσή σας, επισυνάπτεται το .DLL της DotNetZip library, αλλά έχετε την ευχέρεια να χρησιμοποιήσετε όποια εξωτερική βιβλιοθήκη θέλετε
    • Ο κωδικός του archive είναι FirstCall13
    • Η καρτέλα του οφειλέτη θα περιέχει τα τηλέφωνα του οφειλέτη, τις πληρωμές που έχουν γίνει και τα υπόλοιπα στοιχεία της υπόθεσης. Ο τρόπος παρουσίασης αυτών των πληροφοριών (π.χ. Grid), είναι στην κρίση σας
    • Η εφαρμογή θα καλεί το SSIS και θα εισάγει τα δεδομένα στους πίνακες.
    • Η εφαρμογή θα διαβάζει τα δεδομένα προς εμφάνιση από τη βάση δεδομένων
    • Στο αρχείο Γραμμογράφηση αρχείων.xls, θα βρείτε τη γραμμογράφηση των αρχείων
    • Για την σύνδεση μεταξύ των αρχείων θα χρησιμοποιήσετε τα παρακάτω κλειδιά 
        ◦ Το αρχείο των υποθέσεων(Cases) ενώνεται με το αρχείο σχέσεων με το κλειδί υπόθεσης. 
        ◦ Το αρχείο σχέσεων ενώνεται με το αρχείο προσώπων(Person) με το κλειδί προσώπου και το κλειδί οφειλέτη αντίστοιχα. 
        ◦ Το αρχείο προσώπων ενώνεται με το αρχείο τηλεφώνων (Phone) με το κλειδί οφειλέτη. 
        ◦ Το αρχείο υποθέσεων ενώνεται με το αρχείο πληρωμών (Payment) με το κλειδί υπόθεσης. 

Καλή επιτυχία
