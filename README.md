# BTL-TRR2
Đây là bài tập lớn môn Toán rời rạc 2 PTIT: 
🕸️ Phân Tích Cấu Trúc Mạng Lưới Xã Hội
Dự án phân tích và trực quan hóa mạng xã hội bằng Python, sử dụng các thuật toán đồ thị để tính toán các chỉ số quan trọng như PageRank, Betweenness Centrality, và phát hiện cộng đồng (community detection) theo thuật toán Louvain.

📋 Mục Lục

Tính năng

Yêu cầu hệ thống

Cài đặt

Cách sử dụng

Cấu trúc dữ liệu

Các chỉ số phân tích

Dashboard trực quan hóa

Cấu trúc dự án


✨ Tính Năng

✅ Xây dựng đồ thị có hướng (DiGraph) từ dữ liệu quan hệ người dùng

✅ Tính toán PageRank — đo lường mức độ uy tín/ảnh hưởng của từng node

✅ Tính toán Betweenness Centrality — xác định các node đóng vai trò cầu nối

✅ Tính toán Local Clustering Coefficient (LCC) — đo mức độ gom cụm cục bộ

✅ Phát hiện cộng đồng tự động bằng thuật toán Louvain

✅ Xuất Dashboard tổng hợp gồm bản đồ mạng lưới + biểu đồ xếp hạng

```text
social-network-analysis/
|
├── social_network.py    # File chính – toàn bộ logic phân tích & vẽ
└── README.md            # Tài liệu hướng dẫn
