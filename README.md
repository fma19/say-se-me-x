#include <iostream>
#include <cstdlib> // rand() ve srand() için gerekli

int main() {
    // Rastgele sayı üretmek için zamanı kullanalım
    srand(time(0));

    // 1 ile 100 arasında rastgele bir sayı seçelim
    int min = 1;
    int max = 100;
    int randomNumber = min + rand() % (max - min + 1);

    std::cout << "Rastgele seçilen sayı: " << randomNumber << std::endl;

    return 0;
}
