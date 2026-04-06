# Definir el compilador y el estándar C23
CC = gcc
CFLAGS = -std=c23 -Wall -Wextra

# Regla para compilar (Se ejecuta solo con 'make')
all: hello.c
	$(CC) $(CFLAGS) hello.c -o hello.exe

# Regla para ejecutar (Crédito extra: 'make run')
run: all
	.\hello.exe

# Regla para generar el archivo de salida
test: all
	.\hello.exe > output.txt

# Regla para limpiar archivos generados
clean:
	del hello.exe output.txt