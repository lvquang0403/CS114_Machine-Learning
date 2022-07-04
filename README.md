# TÓM TẮT BÁO CÁO ĐỒ ÁN NHẬN DIỆN SẢN PHẨM BÁN LẺ TRONG THANH TOÁN

## Tổng quan:

- INPUT: Là một bức ảnh từ trên chiếu xuống quầy thanh toán với ánh sáng trắng rõ ràng trong đó bao gồm nhiều món hàng không xếp chồng lên nhau trong một khu vực được định sẵn bằng một cái khay hay đường viền màu được chụp từ một camera hoặc điện thoại

- OUTPUT: Là bức ảnh từ input nhưng có các đường viền vuông bao quanh các món hàng có màu xanh,  là món hàng nhận diện được và món và trên các thanh trên cùng được gán nhãn tên của món đồ.


- Dựa trên các nghiên cứu có trước https://arxiv.org/abs/1901.07249

- Thu thập được tổng cộng 13920 tấm ảnh của 94 class là các sản phẩm bán lẻ trong siêu thị

- Pretrain lại Model Yolov4 được kết quả trên tập test: 78,61%

- Pretrain lại Model Faster R-CNN sử dụng framework detectron2 đạt kết quả trên tập test là : 67,15%

## Tóm tắt file:

- ### Detectron2.ipynb: là file training Model Faster R-CNN
- ### ModelYolov4.ipynb: là file training Model Yolov4
- ### 19521571.19522093.19522448.pdf: là file báo cáo đồ án

## DATASET:
+ ### Có 12294 ảnh được train và 12294 file txt chứa nhãn:

File zip: https://drive.google.com/file/d/1kvtTGFa_814G3Ebgiy5guisVEhRGzGD4/view?usp=sharing

Thư mục Drive:https://drive.google.com/drive/u/1/folders/1oddM0E08yIo1ip4pvvVtw_OSfs7RZSp-

+ ### Có 1626 ảnh và 1626 nhãn trong tập test:

File zip:
https://drive.google.com/file/d/https://drive.google.com/file/d/1-mDmUsh9SZzKAvMFt4vejvU7XcejQpB7/view?usp=sharing

Thư mục Drive:
https://drive.google.com/drive/folders/1Fb9xuLE9OfW93-lSh2dNbVmdP9OVskKm?usp=sharing

Github:https://github.com/truyenaaa123/CS114.L22.KHCL/tree/main/Project/Data/data_test


- ### 322 video:

Folder Drive: https://drive.google.com/drive/folders/1-5a_xK7WE-6wG36dslxDErLpAT56mUGq?usp=sharing

- ### Demo:
link colab: https://colab.research.google.com/drive/1uWvLYvQW3oP_7gkllUi5GfRF6FVL8PLe?usp=sharing&fbclid=IwAR1pRPtrdxxlglFNzscXMxsQ4iGBUA5Xysxz_aNVougOJE71pq-2y3PSvcw#scrollTo=pnwZVwADyoV3

## Những cập nhật thay đổi so với lần báo cáo vần đáp trước

+ Đã train và đánh giá kết quả model Yolov4 và Faster R-CNN
+ Tăng cường dữ liệu thêm 3107 ảnh có chứa từ 3-6 vật
+ Hoàn thành cơ bản một cái demo trên colab