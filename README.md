# MHE-PJATK

#Knapsack Problem - NP COMPLETE


Knapsack Problem czy też Problem plecakowy polega na tym że chcemy otrzymać taki plecak,
który będzie miał jednocześnie największa wartość jednak utrzymał określaną przez nas podaną pojemność.

W rozwiązaniu musimy dobrać taki podzbiór z zbiory elementów o podanej wadze i wartości by wartość była jak najwięskza przy podanej pojemności plecaka.


Przykład :

Przedmiot  Waga  Wartość
  ------------------------
      1       25      40
      2       42      68
      3       20      56
  ------------------------
  Pojemność plecaka:  50
  
Pseudokod:

void probuj(int k)
{
    if (k < n) probuj(k + 1);
    if (można dołożyć przedmiot k do plecaka)
    {
        zapisz, że Alibaba zabiera przedmiot k;
        if (wartość wynoszonej części skarbu jest wyższa)
            zapamiętaj nowy zestaw i jego wartość;
        if (k < n) probuj(k + 1);
        usuń zapis, że Alibaba zabiera przedmiot k;
    }
} 


