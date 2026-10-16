```C
/**
 * @author Nasser AHAMED
 * @date 8/10/2026
 * @description Implémentation d'un algorithme de QuickSort, avec un pivot.
 * Les éléments inférieur à ce pivot passe à gauche
 * et on fait un appel récursive sur le nouvelle interval.
 */
void iqsort0(int *a, int n) {
    
    int i, j;
    
    // Si taille du tableau <= 1 on s'arrête
    if (n <= 1)
        return;
    
    // a[0] est choisi comme pivot
    // 'j' garde la trace de la frontière des éléments strictement inférieurs au pivot
    for (i = 0, j = 0; i < n; i++) 
        if (a[i] < a[0])
            // On incrémente la frontière et on échange l'élément trouvé vers la zone gauche
            swap(++j, i, a);
            
    // On insère le pivot à sa place définitive à l'indice 'j'
    // Tous les éléments avant 'j' sont < au pivot, tous ceux après sont >= pivot
    swap(0, j, a);
    
    // Appel récursif sur le sous-tableau gauche (les j éléments avant le pivot)
    iqsort0(a, j);
    
    // Appel récursif sur le sous-tableau droit (les éléments restants après le pivot)
    // On décale le pointeur de début (a + j + 1) et on ajuste la taille restante
    iqsort0(a + j + 1, n - j - 1);
}
```