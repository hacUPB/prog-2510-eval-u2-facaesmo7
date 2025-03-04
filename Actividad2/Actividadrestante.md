

## 3. 

### 
A continuación,  los tipos de datos en  lenguajes de programación:

| Tipo de Dato  | C       | Java     | Python   |
|--------------|---------|---------|---------|
| Entero      | `int`   | `int`   | `int`   |
| Decimal     | `float` | `double` | `float` |
| Booleano    | `bool`  | `boolean` | `bool`  |
| Caracter    | `char`  | `char`   | `str` (1 caracter) |
| Cadena      | `char[]` o `string` | `String` | `str` |



## 4. 
tabla de resultados:

| Nombre de la Variable | Abreviación | Características |
|----------------------|------------|----------------|
| Número entero       | `int`      | Valores enteros, rango depende del lenguaje |
| Número decimal      | `float`    | Valores con punto flotante |
| Booleano           | `bool`     | `True` o `False` |
| Texto              | `string`   | Secuencia de caracteres |

## 5. Se almacena la información cada 10 segundos durante 24 horas. Calcula cuánto espacio total se requiere en memoria para almacenar estos datos. Describe el procedimiento y muestra el resultado final.

### Cálculo del espacio en memoria

- **Entero (`int`)**: 4 bytes
- **Flotante (`float`)**: 4 bytes
- **Booleano (`bool`)**: 1 byte
- **Texto (10 caracteres, `string`)**: 10 bytes (1 byte por carácter)

Espacio total por registro: 4 + 4 + 1 + 10 = 19 bytes

Total de registros en 24 horas:

\[ \frac{24 \times 60 \times 60}{10} = 8640 \] registros

Espacio total requerido:

\[ 19 \times 8640 = 164,160 \] bytes (aproximadamente 160.3 KB)

## 6. Conclusión
 Este ejercicio permitió comprender cómo se almacenan diferentes tipos de datos en la memoria y la importancia de aprovechar el  espacio en los programas.
