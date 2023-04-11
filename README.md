#include <stdio.h>

// Function to check if a number is composite
int isComposite(int n) {
    int i;
    for(i=2; i<=n/2; i++) {
        if(n%i == 0) {
            return 1; // It is a composite number
        }
    }
    return 0; // It is not a composite number
}

int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);
    
    if(isComposite(n)) {
        printf("%d is a composite number.", n);
    }
    else {
        printf("%d is not a composite number.", n);
    }
    
    return 0;
}
Footer
