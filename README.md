int main() {
    char text[100];
    
    printf("Bir kelime veya cumle girin: ");
    fgets(text, sizeof(text), stdin);
    text[strcspn(text, "\n")] = '\0';  // İstenmeyen yeni satır karakterini kaldırın
    
    int length = strlen(text);
    
    printf("Metnin uzunlugu: %d\n", length);
    
    return 0;
}
