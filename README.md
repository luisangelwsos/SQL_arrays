# SQL_arrays
como usar arrays en sql para anidar datos
Puedes hacer cosas muy útiles con los arrays, como las siguientes:

Calcular la cantidad de elementos con ARRAY_LENGTH(<array>)
Anular la duplicación de elementos con ARRAY_AGG(DISTINCT <field>)
Ordenar elementos con ARRAY_AGG(<field> ORDER BY <field>)
Limitar ARRAY_AGG(<field> LIMIT 5)

# SQL_structs

Un STRUCT de SQL es básicamente un contenedor de otros campos de datos que pueden ser de distintos tipos. La palabra "struct" significa "estructura de datos". Recuerda el ejemplo que mencionamos antes:
STRUCT("Rudisha" as name, [23.4, 26.3, 26.4, 26.1] as splits) AS runner
A los STRUCTS se les da un alias (como “runner” en el ejemplo anterior) y podemos entenderlos como una tabla dentro de una tabla principal.
Es necesario descomprimir los STRUCTS (y los ARRAYS) para poder usar sus elementos. Incluya UNNEST() junto al nombre del struct o del campo del struct que es un array para descomprimirlo y compactarlo.
