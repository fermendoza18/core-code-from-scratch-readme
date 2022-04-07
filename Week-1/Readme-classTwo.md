# Your date of birth in the matrix?

## Convert Decimal to Binary

| 1024  |  512  |   256 | 128  |  64  |  32 | 16  | 8   |  4 |   2 |  1  |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
| 2^10 | 2^9 | 2^8 | 2^7  |  2^6  |  2^5  | 2^4  | 2^3  | 2^2  | 2^1  | 2^0 |
| 1  | 1  | 1  | 1  |  1 |  0  | 0  | 1  | 1  | 1  | 0 |

Sumamos todas las posiciones con 1 para encontrar el número decimal.

- Binary: 11111001110
- Decimal: 1998

------------
    
# Create a program to add two numbers given by the user
    .data
    	      number1: .asciiz "\nIngrese el primer numero: "
    	      number2: .asciiz "\nIngrese el segundo numero: "
    	      result_message: .asciiz "\nEl resultado es: "
      .text
    	      main:
                  # Imprime en consola el string numero1
                  li $v0, 4
                  la $a0, number1
                  syscall
    
                  # Recibe el input del usuario
                  li $v0, 5
                  syscall
    
                  # Guarda el input del usuario en $t0
                  move $t0, $v0
    
                  # Imprime en consola el string numero2
                  li $v0, 4
                  la $a0, number2
                  syscall
    
                  # Recibe el input del usuario
                  li $v0, 5
                  syscall
    
                  # Guarda el input del usuario en $t1
                  move $t1, $v0
                  
                  # Efectua la suma de los dos numeros y lo guarda en $t2
                  add $t2, $t0, $t1
                  
                  # Imprime el string que contiene add_message
                  li $v0, 4
                  la $a0, result_message
                  syscall
                  
                  # Imprime el entero resultado de la suma
                  li $v0, 1
                  move $a0, $t2
                  syscall
                  
------------

# Create a program that display your name

    .data
    	      say_my_name: .asciiz "\nMi nombre es: Fernando Mendoza \n"
      .text
    	      main:
            
                  # Imprime en consola el string say_my_name
                  li $v0, 4
                  la $a0, say_my_name
                  syscall
