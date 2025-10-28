#include <stdio.h>

int main() {
    int A, B, R;

    printf("Entrez deux entiers positifs : ");
    scanf("%d %d", &A, &B);

    // Algorithme d’Euclide
    while (b != 0) {
        R = A % B;
        A = B;
        B = R;
    }

    printf("Le PGCD est : %d\n", A);

    return 0;
}
