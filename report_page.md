## Pipeline đã chạy
- Sinh dữ liệu text sentiment giả lập (random, 300 mẫu) → TF-IDF (1-2 grams) → LogisticRegression (max_iter=500) → evaluate.
- Seed = 42 để đảm bảo reproducibility.

## Kết quả
- **Accuracy**: 1.0, **Macro-F1**: 1.0 (xem `results/lab0_metrics.json`).
- Train: 240 mẫu, Test: 60 mẫu, Vocab size: 112.
- Confusion matrix: hoàn hảo (không có lỗi phân loại).

## Vấn đề gặp phải + cách xử lý
- Không gặp vấn đề nào. Setup môi trường chạy thành công.
- Môi trường: Python 3.13.5, NumPy 2.1.3, Pandas 2.2.3, sklearn 1.6.1.

## Ghi chú
- Dữ liệu random chỉ để kiểm tra setup, không dùng để so sánh mô hình thật.
- Tất cả 6 unit tests đều PASS.

## không phải code e sai đâu mà cô :((