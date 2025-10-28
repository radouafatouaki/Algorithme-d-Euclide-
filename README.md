#include <stdio.h>

int main() {
    int A, B, R;  // Déclaration des variables

    // Saisie des deux nombres
    printf("Donner le premier nombre A : ");
    scanf("%d", &A);

    printf("Donner le deuxième nombre B : ");
    scanf("%d", &B);

    printf("\nDébut du calcul du PGCD\n\n");

    // Boucle de l'algorithme d'Euclide
    while (B != 0) {
        R = A % B;   // Calcul du reste
        printf("A = %d, B = %d, reste = %d\n", A, B, R);  // Affichage des valeurs à chaque étape

        A = B;       // On remplace A par B
        B = R;       // On remplace B par le reste
    }

    // Fin de la boucle
    printf("\nLe PGCD est : %d\n", A);

    return 0;
}
