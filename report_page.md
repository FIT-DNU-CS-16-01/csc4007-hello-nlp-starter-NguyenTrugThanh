# Lab0 — 1-page report (Hello NLP, random data)

## Pipeline đã chạy
- Sinh dữ liệu text sentiment giả lập (random, 300 mẫu) → TF-IDF (1-2 grams) → LogisticRegression (max_iter=500) → evaluate.
- Sử dụng stratified train_test_split, seed=42 để đảm bảo reproducibility.

## Kết quả
- **Accuracy**: 1.0, **Macro-F1**: 1.0 (xem `results/lab0_metrics.json`).
- Train: 240 mẫu, Test: 60 mẫu, Vocab size: 112.
- Confusion matrix: hoàn hảo (không có lỗi phân loại).

## Vấn đề gặp phải + cách xử lý
- Không gặp vấn đề nào. Code chạy thành công từ lần đầu.
- Anti-leakage: vectorizer chỉ fit trên train set, không fit trên test set.

## Ghi chú
- Dữ liệu random chỉ để kiểm tra setup, không dùng để so sánh mô hình thật.
- Tất cả 6 unit tests đều PASS (bao gồm test_reproducibility, test_no_leakage_vectorizer).