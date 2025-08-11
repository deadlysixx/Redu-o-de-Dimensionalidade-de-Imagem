# Reducao-de-Dimensionalidade-de-Imagem
Este projeto contém um script em Python que converte uma imagem colorida no formato **PPM (P3)** para:  - Imagem em tons de cinza (escala 0-255) - Imagem binarizada (preto e branco, valores 0 e 255)

## Como usar

1. Coloque uma imagem no formato PPM texto (`P3`) na mesma pasta do script, com o nome `imagem.ppm`.
2. Execute o script:

```bash
python converter.py
Serão gerados dois arquivos:

imagem_gray.pgm — imagem em tons de cinza

imagem_bin.pgm — imagem binarizada (preto e branco)

Você pode abrir esses arquivos com visualizadores que suportam PGM, como GIMP ou IrfanView.

Estrutura do código
ler_ppm(caminho) — lê a imagem PPM e retorna largura, altura, valor máximo e pixels RGB.

rgb_para_gray(pixels) — converte RGB para tons de cinza usando fórmula ponderada.

binarizar(pixels_gray, limiar=128) — converte tons de cinza para binário com threshold.

salvar_ppm_gray e salvar_ppm_bin — salvam as imagens em formato PGM.
```

## Requisitos
- Python 3 <br>
- Imagem de entrada em formato PPM (P3)
