# Сжатие и ускорение LLM путем квантизации весов и активаций в Int8

Репозиторий содержит код Домашней работы для построения квантизованного линейного слоя, веса которого хранятся в Int8, а во время расчета `forward` выполняется квантизация активаций. Данный линейный слой в дальнейшем используется в LLM с целью уменьшения потребления памяти и ее ускорения. 

Для более быстрых расчетов предлагается использовать triton kernels от bitsandbytes.

Описание репозитория:

- quantization_8bit.ipynb - jyputer notebook, в котором содержится весь код.
- bnbtriton - папка, в которой содержится код triton kernels, реализующих операцию квантизации и матричного умножения в Int8 с одновременной деквантизацией.
