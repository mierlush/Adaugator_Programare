Ziua 1
Calcularea Mediei:
•	Scrie un program care primește două numere de la utilizator și afișează media lor
Rezolvare:

#include <iostream>
using namespace std;
int main() 
{
    float nr1, nr2;
    cout << "introdu primul număr: ";
    cin >> nr1;
    cout << "introdu al doilea număr: ";
    cin >> nr2;
    float media = (nr1 + nr2) / 2;
    cout << "Media numerelor este: " << media / 2 << endl;
    return 0;
}

![image](https://github.com/mierlush/Adaugator_Programare/assets/163460760/26d70b1b-fd1a-4f24-adb1-7c38c1c1d813)

Joc de Ghicire:
•	Creează un program care generează un număr aleatoriu între 1 și 100. Utilizatorul încearcă să ghicească numărul și primește indicii dacă răspunsul său este prea mare sau prea mic.
Rezolvare:

#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    srand(time(nullptr));
    int numar_aleatoriu = rand() % 100 + 1;
    int ghicire;
    cout << "Incearca sa ghicesti numarul intre 1 si 100." << endl;
    while (true) {
        cout << "Introdu un numar: ";
        cin >> ghicire;
        if (ghicire == numar_aleatoriu) {
            cout << "Felicitari! Ai ghicit numarul." << endl;
            break;
        } else if (ghicire < numar_aleatoriu) {
            cout << "Prea mic! Incearca din nou." << endl;
        } else {
            cout << "Prea mare! Incearca din nou." << endl;
        }
    }
    return 0;
}
Zaruri
•	Implementează un joc de zaruri în care utilizatorul încearcă să ghicească suma a două zaruri aruncate. Dacă suma este 7 sau 11, utilizatorul câștigă; dacă este 2, 3 sau 12, utilizatorul pierde; în orice alt caz, jocul continuă.

Rezolvare:
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    srand(time(nullptr));
    cout << "Bine ai venit la jocul de zaruri!" << endl;
    while (true) {
        cout << "Apasa o tasta pentru a arunca zarurile...";
        getchar();
        int suma = rand() % 6 + 1 + rand() % 6 + 1;
        cout << "Suma este " << suma << endl;
        if (suma == 7 || suma == 11)
            cout << "Felicitari! Ai castigat!" << endl;
        else if (suma == 2 || suma == 3 || suma == 12)
            cout << "Ai pierdut! Mai incearca o data." << endl;
        else
            cout << "Nu ai castigat sau pierdut. Mai incearca o data." << endl;
        if (suma == 7 || suma == 11 || suma == 2 || suma == 3 || suma == 12)
            break;
    }
    return 0;
}


Ziua 2
Verificare Paritate:
•	Solicită utilizatorului să introducă un număr și afișează un mesaj care indică dacă numărul este par sau impar.
Rezolvare:

#include <iostream>
using namespace std;

int main() {
    int numar;
    cout << "Introdu un numar: ";
    cin >> numar;
    if(numar % 2 == 0) {
        cout << "Numarul este par." << endl;
    } else {
        cout << "Numarul este impar." << endl;
    }
    return 0;
}

 ![image](https://github.com/mierlush/Adaugator_Programare/assets/163460760/98772f9a-7839-45d1-95ee-f3eccca5a61d)


Calcularea Puterii:
•	Solicită utilizatorului să introducă o bază și un exponent și calculează rezultatul ridicării la putere.
Rezolvare
#include <iostream>
using namespace std;

int main() {
    int baza, exponent, rezultat = 1;
    cout << "Introdu o baza: ";
    cin >> baza;
    cout << "Introdu un exponent: ";
    cin >> exponent;
    for (int i = 0; i < exponent; i++) {
        rezultat *= baza;
    }
    cout << "Rezultatul ridicarii la putere este: " << rezultat << endl;
    return 0;
}

 ![image](https://github.com/mierlush/Adaugator_Programare/assets/163460760/8cd9e0f1-57ef-4952-958f-dbc17e694c9b)

Gestionarea Intrărilor Utilizatorului:
Rezolvare =NULL

Ziua 3
Compararea Numerelor:
•	Ia trei numere de la utilizator și afișează cel mai mare dintre ele.
Rezolvare:

#include <iostream>
using namespace std;

int main() {
    int numar1, numar2, numar3;
    cout << "Introdu primul numar: ";
    cin >> numar1;
    cout << "Introdu al doilea numar: ";
    cin >> numar2;
    cout << "Introdu al treilea numar: ";
    cin >> numar3;
    int celMaiMare = numar1;
    if (numar2 > celMaiMare)
        celMaiMare = numar2;
    if (numar3 > celMaiMare)
        celMaiMare = numar3;
    cout << "Cel mai mare numar este: " << celMaiMare << endl;
    return 0;
}
 
![image](https://github.com/mierlush/Adaugator_Programare/assets/163460760/45a1afed-69ab-45d5-8251-f0c5bb0b80bf)
