# Utilize PoSHAP to explain model's prediction on biological sequences

Tất cả các phần code train, test và sinh biểu đồ phân tích PoSHAP đều nằm trong các Notebook prefix main, chia 3 notebook cho 3 bộ dữ liệu, và 1 notebook XGBoost thử nghiệm PoSHAP trên mô hình khác.

Kiến trúc thư mục bao gồm:

- Data: Chứa dữ liệu train, test, validation của 3 bộ dữ liệu
- Dep: Matrix phân tích quan hệ có ý nghĩa giữa các thành phần, lưu dưới dạng .npy
- DependenciesSpreadsheet: Đầu ra quan hệ có ý nghĩa dưới dạng .csv
- Images: Chứa các hình ảnh đã sinh trong quá trình phân tích
- Model: Chứa Keras model phục vụ cho việc load
- Poshap: Matrix lưu SHAP trên từng chỉ số (index) phục vụ cho việc sinh phân tích PoSHAP
- Reg_SHAP (deprecated): Matrix tổng quan SHAP theo vị trí-thành phần, hữu ích khi sinh heatmap tổng quan
