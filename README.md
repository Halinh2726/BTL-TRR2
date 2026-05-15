# Social Network Analysis Dashboard

## Giới thiệu
Dự án này xây dựng một hệ thống phân tích mạng xã hội bằng Python sử dụng:

- NetworkX để mô hình hóa đồ thị
- Pandas để xử lý dữ liệu
- Matplotlib + Seaborn để trực quan hóa
- python-louvain để phát hiện cộng đồng (Community Detection)

Chương trình mô phỏng mạng xã hội dạng directed graph (đồ thị có hướng), sau đó phân tích các chỉ số quan trọng như:

- PageRank → Độ uy tín / mức ảnh hưởng
- Betweenness Centrality → Vai trò cầu nối
- Local Clustering Coefficient (LCC) → Mức độ gom cụm
- Community Detection (Louvain) → Phân cụm cộng đồng


# Nội dung dự án

Project gồm:

- File báo cáo PDF
- File Jupyter Notebook (.ipynb)

Notebook chứa toàn bộ:
- Source code
- Phân tích dữ liệu
- Trực quan hóa dashboard


# Demo Dashboard

Các thành phần trực quan gồm:

1. Bản đồ kết nối mạng xã hội
- Hiển thị toàn bộ quan hệ giữa các user
- Node càng lớn → độ ảnh hưởng càng cao
- Màu sắc thể hiện cộng đồng

2. Top 8 PageRank
- Xếp hạng các node có độ uy tín cao nhất

3. Top 8 Betweenness
- Xếp hạng các node đóng vai trò trung gian quan trọng


# Công nghệ sử dụng

- Python 3.x
- NetworkX
- Pandas
- Matplotlib
- Seaborn
- python-louvain
- Jupyter Notebook


# Cài đặt thư viện

pip install networkx matplotlib pandas seaborn python-louvain


# Cách chạy project

## Chạy bằng Jupyter Notebook

jupyter notebook

Sau đó mở file:

social_network_analysis.ipynb


## Hoặc chạy bằng Google Colab

Upload file notebook lên Google Colab và chạy từng cell.


# Cấu trúc chương trình

## create_social_graph()

Khởi tạo directed graph và thêm các mối quan hệ giữa user.


## get_analytics(G)

Tính toán:

- PageRank
- Betweenness Centrality
- Clustering Coefficient
- Louvain Community Detection

Sau đó trả về DataFrame chứa toàn bộ dữ liệu phân tích.


## draw_dashboard(G, df, partition)

Sinh dashboard trực quan gồm:

- Network Graph
- Biểu đồ PageRank
- Biểu đồ Betweenness

Có xử lý:
- chống chồng node
- cạnh cong cho quan hệ 2 chiều
- scale node theo PageRank
- tô màu theo community


# Ý nghĩa các chỉ số

| Chỉ số | Ý nghĩa |
|--------|----------|
| PageRank | Độ uy tín / sức ảnh hưởng |
| Betweenness | Mức độ làm cầu nối |
| LCC | Mức độ liên kết cục bộ |
| Community | Nhóm xã hội / cụm cộng đồng |


# Kết quả đầu ra

## Console

In bảng dữ liệu phân tích:

User | PageRank | Betweenness | LCC | Community


## Dashboard

Hiển thị dashboard trực quan bằng matplotlib.


# Google Colab

Link Google Colab:

https://colab.research.google.com/

Nếu có notebook riêng:
[Open In Colab](https://colab.research.google.com/drive/1CiOGfiVWAXpuOEFP49txISLDuXTaAP9s?usp=sharing)



# Tác giả

Project phục vụ mục đích:
- học tập
- nghiên cứu Social Network Analysis
- trực quan hóa đồ thị mạng xã hội
