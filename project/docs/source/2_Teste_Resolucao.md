# Teste 2
## Introdução à Programação

#### 1) [2,5 Valores] Qual o output deste programa?

        #include <stdio.h>
        #define DIM 5
        void mostrar(int[][DIM], int, int);
        void inicializar(int[][DIM], int, int);
        int main()
        {
            int matriz[DIM][DIM];
            int linhas =3, colunas=4;
            inicializar(matriz,linhas,colunas);
            mostrar(matriz,linhas,colunas);
            printf("\n\n");
            colunas=2;
            inicializar(matriz,linhas,colunas);
            mostrar(matriz,linhas,colunas);
            printf("\n\n");
            return 0;
        }
        void inicializar(int m[][DIM], int nl, int nc)
        {
            int i, j, k=0;
            for (i = 0; i < nl; i++)
                for (j = 0; j < nc; j++)
                    m[i][j] = k++;
        }
        void mostrar(int m[][DIM], int nl, int nc)
        {
            int i, j;
            for (i = 0; i < nl; i++)
            {
                for (j = 0; j < nc; j++)
                    printf("%2d ", m[i][j]);
                printf("\n");
            }
        }

---
