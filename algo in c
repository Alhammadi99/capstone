#include <stdio.h>
#include <string.h>

void compressRLE(char* data) {
    int length = strlen(data);
    for (int i = 0; i < length; i++) {
        int count = 1;
        while (i < length - 1 && data[i] == data[i + 1]) {
            count++;
            i++;
        }
        printf("%c%d", data[i], count);
    }
}

int main() {
    char data[] = "AAABBBCCCCDDDDEEEE";
    printf("Original Data: %s\n", data);
    printf("Compressed Data: ");
    compressRLE(data);
    return 0;
}
