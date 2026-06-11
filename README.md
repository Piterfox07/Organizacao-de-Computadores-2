Simulador de Memoria Cache (C++)
Este projeto implementa um simulador de cache com mapeamento direto e mapeamento por conjunto.
Como compilar
No terminal, execute:
```powershell
cl /EHsc cache_simulator.cpp /Fe:cache_simulator.exe
```
ou com `g++`:
```powershell
g++ -std=c++17 cache_simulator.cpp -o cache_simulator.exe
```
Como usar
```powershell
cache_simulator.exe --cache-size 1024 --block-size 16 --assoc 2 --addr-bits 16 --input Memoria1.txt --politica LRU
```
Se nenhum parametro for passado, o programa entra em modo interativo.
Formato do arquivo de entrada
Um endereco por linha.
Pode ser decimal ou hexadecimal (`0x...`).
Linhas iniciadas com `#` sao ignoradas.
