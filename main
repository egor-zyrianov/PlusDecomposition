#include <stdio.h>
#define N 5

int rip(int count, int start, int step){
    for (int i = step-1; i > 0; i--){
        int bully = start; 
        printf("\n%d", start);
        while (bully < N){
            printf("+%d", i);
            bully += i;
            if (bully < N && i > 1){count = rip(count, bully, i);}
        }
        if (bully == N){count++;printf("=%d", bully);}
    }
    return count;
}

int main() {
    
    int count = 0;
    for (int i = 1; i < N; i++){
        int bully = 0;
        while (bully < N){
            bully += i;
            if (bully < N){count = rip(count, bully, i);}
        }
        if (bully == N){count++; 
        printf("\n%d*%d=%d", i,bully/i, bully);}
    }
    
    printf("\noverall: %d", count);
    return 0;
}
