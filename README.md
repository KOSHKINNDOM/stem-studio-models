# Модели K1RO Stem Studio

Раздача весов для программы K1RO Stem Studio: ONNX-графы, которые программа сама скачивает при первом запуске
по манифесту `stem-studio.json` (лежит в раздаче моделей K1RO AI Voice вместе с общими моделями).
Здесь — только модели, которых нет у AI Voice.

| Файл | Что это |
|---|---|
| `models__separation__sw-6stem.matmul.fp16.onnx` | BS-RoFormer SW, 6 стемов — TensorRT-RTX (NVIDIA) |
| `models__separation__sw-6stem.mha.fp16.onnx` | то же — WebGPU (любая видеокарта, Mac) |
| `models__separation__sw-6stem.mha.onnx` | то же — процессор (fp32) |
| `models__separation__drumsep-6s.matmul.fp16.onnx` | MDX23C DrumSep aufr33 + jarredou, 6 стемов (бочка, рабочий, томы, хай-хэт, райд, крэш) — TensorRT-RTX |
| `models__separation__drumsep-6s.mha.fp16.onnx` | то же — WebGPU (граф тот же, что у TensorRT: у MDX23C нет внимания) |
| `models__separation__drumsep-6s.mha.onnx` | то же — процессор (fp32) |
| `models__separation__mega53-groups.matmul.fp16.onnx` | MVSep Mega 53, шины: клавишные, струнные, духовые, баян — ствол и четыре головы, маски сложены в графе; TensorRT-RTX (внимание в fp32) |
| `models__separation__mega53-groups.mha.fp16.onnx` | то же — WebGPU |
| `models__separation__mega53-groups.mha.onnx` | то же — процессор (fp32) |
