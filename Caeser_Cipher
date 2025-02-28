#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];
    int ch;

    while(1) {
        printf("---Ceaser Cipher---\n");
        printf("1. ENCRYPTION\n");
        printf("2. DECRYPTION\n");
        printf("3. EXIT\n");
        printf("Enter your choice: \n");
        scanf("%d", &ch);

        switch (ch) {
            case 1:
                printf("---ENCRYPTION---\n");
                printf("Plaintext: ");
                getchar();
                fgets(str, 100, stdin);

                {
                    int key;
                    printf("Enter the Key:");
                    scanf("%d", &key);
                    if(key < 0 || key > 25) {
                        printf("\nInvalid Key");
                        break;
                    }

                    for (int i = 0; str[i] != '\0'; ++i) {
                        if (isalpha(str[i])) {
                            char offset = isupper(str[i]) ? 'A' : 'a';
                            char new_char = (str[i] - offset + key) % 26 + offset;
                            str[i] = new_char;
                        }
                    }
                    printf("Ciphertext: %s\n", str);
                }
                break;

            case 2:
                printf("---DECRYPTION---\n");
                printf("Ciphertext: ");
                getchar();
                fgets(str, 100, stdin);

                {
                    int key;
                    printf("Enter the Key:");
                    scanf("%d", &key);
                    if(key < 0 || key > 25) {
                        printf("\nInvalid Key");
                        break;
                    }

                    for (int i = 0; str[i] != '\0'; ++i) {
                        if (isalpha(str[i])) {
                            char offset = isupper(str[i]) ? 'A' : 'a';
                            char new_char = (str[i] - offset - key + 26) % 26 + offset;
                            str[i] = new_char;
                        }
                    }
                    printf("Plaintext: %s\n", str);
                }
                break;

            case 3:
                printf("Exiting...\n");
                return 0;

            default:
                printf("INVALID");
                break;
        } 
    }

    return 0;
}
