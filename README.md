# JarHandler

JarHandler - это утилита для шифрования и дешифрования JAR-файлов с использованием алгоритма AES. Этот инструмент обеспечивает безопасное хранение ваших JAR-файлов, делая их недоступными для неавторизованных пользователей.

# Возможности

Генерация AES-ключа.
Шифрование JAR-файла и сохранение его в формате .dat.
Дешифрование зашифрованного файла.
Повторное шифрование перед запуском.
Требования
Java 8 или выше
Установка
Склонируйте репозиторий или скачайте исходный код.
Скомпилируйте исходный код:
 ```bash
javac -d bin src/org/example/SecureJarHandler.java
```

# Шаг 1: Генерация ключа и шифрование JAR-файла

Запустите программу, чтобы зашифровать ваш JAR-файл:
```bash
java -cp bin org.example.SecureJarHandler
```

# Шаг 2: Проверка файлов

После выполнения программы, на вашем компьютере будут созданы следующие файлы:

```
test.jar - исходный JAR-файл.
encrypted_file.dat - зашифрованный JAR-файл.
secret.key - файл, содержащий сгенерированный AES-ключ.
re_encrypted_test.jar - повторно зашифрованный JAR-файл.
```

# Шаг 3: Настройка путей

Убедитесь, что пути к файлам в коде соответствуют вашим текущим директориям:

```bash
String jarPath = "C://Users/fecur/Desktop/byte/test.jar";
String encryptedPath = "C://Users/fecur/Desktop/byte/encrypted_file.dat";
String keyPath = "C://Users/fecur/Desktop/byte/secret.key";
String reEncryptedPath = "C://Users/fecur/Desktop/byte/re_encrypted_test.jar";
```
