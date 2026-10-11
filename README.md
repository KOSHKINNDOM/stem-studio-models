# Модели K1RO Stem Studio

Раздача весов для программы K1RO Stem Studio: ONNX-графы, которые программа сама скачивает при первом запуске
по манифесту `stem-studio.json` (лежит в раздаче моделей K1RO AI Voice вместе с общими моделями).
Здесь — только модели, которых нет у AI Voice.

| Файл | Что это |
|---|---|
| `models__separation__sw-6stem.matmul.fp16.onnx` | BS-RoFormer SW, 6 стемов — TensorRT-RTX (NVIDIA) |
| `models__separation__sw-6stem.mha.fp16.onnx` | то же — WebGPU (любая видеокарта, Mac) |
| `models__separation__sw-6stem.mha.onnx` | то же — процессор (fp32) |
