# VikoStud_uzd1
https://leetcode.com/problems/valid-palindrome/
#include  <iostream>

using namespace std;
bool is_palindrome(string text)
{
    for (int i = 0; i < text.length() / 2;i++)
        if (text[i] != text[text.length() -i -1])
            return false;
    return true;
}
int main(){
    string test1 = "amanaplanacanalpanama";
    string test2 = "hamburger";
    string test3 = "dogeeseseegod";
    
    if (is_palindrome(test1))
        cout << test1 << "  ==> is a palindrome" << endl;
    else
        cout << test1 <<" ==> is not a palindrome" << endl;

    if (is_palindrome(test2))
        cout << test2 << "  ==> is a palindrome" << endl;
    else
        cout << test2 <<" ==> is not a palindrome" << endl;
                                                          


Problema-patikrinti ar simboliu seka yra palindromas.
Analizė:
sukursime cikla kuriame kintamasis i simbolizuoja simbolių rinkinio pradžią ir yra 0 ir kiekviena karta ciklui prasidejus is naujo prie kintamojo prisideda 1, o simbolių rinkinio pabaiga atitinka text[text.length() -i -1], cikla nutrauksime tuomet kai pasieksime zodzio viduri .tuomet palyginsim kiekviena raidę simbolių rinkinio pradzioje su raide
simbolių rinkinio pabaigoje ir jeigu jos nesutaps funkcija grazins false, jeigu iki simbolių rinkinio vidurio visos raidės sutapo funkcija gražins true.
naudosime bool is_palindrome funkcija 
naudojami kintamieji-
i= 0;

funckijos įvestis bus simboliu eilute(angl. String) 
išvestis true/false(angl boolean).

algoritmo projektavimas 
sukurti funkcija kuri kiekviena cikla prideda prie kintamojo 1
sukurti funkcija kuri palygina raides žodžio pradžioje su raidėmis žoždio pabaigoje ir neatitikmenų atveju meta false, kitu atveju meta true.
sukursime keleta skirtingu simbolių eilučių- string pora palindromų bei viena ne palindromą.
perduosime kiekviena string funkcijai bool_is palindrome patikrinti .


