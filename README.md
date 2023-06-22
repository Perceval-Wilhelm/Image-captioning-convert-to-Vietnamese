<p align="center">
   <a href="https://www.uit.edu.vn/">
      <img src="https://i.imgur.com/WmMnSRt.png" border="none">
   </a>
</p>
<h1 align="center">
    CS114.N11.KHCL - Máy Học
</h1>

## [BẢNG MỤC LỤC](#top)
* [Giới thiệu môn học](#giới-thiệu-môn-học)
* [Thông tin các thành viên](#thông-tin-về-các-thành-viên-nhóm)
* [Mô tả bài toán](#mô-tả-bài-toán)
* [Mô tả bộ dữ liệu](#mô-tả-bộ-dữ-liệu)
* [Mô tả thuật toán](#mô-tả-thuật-toán)
* [Đánh giá](#đánh-giá)
* [Kết quả](#kết-quả)

## [GIỚI THIỆU MÔN HỌC](#top)
* **Tên môn học:** Máy học - Machine Learning
* **Mã môn học:** CS114
* **Mã lớp:** CS114.N11.KHCL
* **Năm học:** HK1 (2022 - 2023)
* **Giảng viên:**
<ul>
      <ul>
         <li> PGS-TS. Lê Đình Duy - duyld@uit.edu.vn </li>
         <li> Ths. Phạm Nguyễn Trường An - truonganpn@uit.edu.vn </li>
      </ul>
</ul>

## [THÔNG TIN VỀ CÁC THÀNH VIÊN NHÓM](#top)
| STT    | MSSV          | Họ và Tên                |Vai trò    | Github                                          | Email                   |
| :----: |:-------------:| :-----------------------:|:---------:|:-----------------------------------------------:|:-------------------------:
| 1      | 20521546      | Lê Tấn Lộc               |Trưởng nhóm|[leetnlok](https://github.com/leetnlok)          |20521546@gm.uit.edu.vn   |
| 2      | 20520934      | Bùi Quốc Thịnh           |Thành viên |[sirrtt](https://github.com/sirrtt)              |20520278@gm.uit.edu.vn   |
| 3      | 20520313      | Nguyễn Hồng Anh Thư      |Thành viên |[thuwpink](https://github.com/thuwpink)          |20520313@gm.uit.edu.vn   |

## [MÔ TẢ BÀI TOÁN](#top)
* **Tên đồ án:** Image Captioning
* **Tóm tắt đồ án:** 

Phát triển một hệ thống máy tính có thể hiểu được thế giới thị giác và giao tiếp với chúng ta bằng ngôn ngữ là một trong những mục tiêu lớn của trí tuệ nhân tạo. Để hiện thực hóa giấc mơ này, vô số bài toán đã được đặt ra, trong đó có Image Captioning. Bài toán này nhận đầu vào là một hình ảnh và cố gắng sinh ra một câu mô tả bằng ngôn ngữ tự nhiên cho ảnh đó.
            
Hiện nay, phương pháp tiếp cận giải quyết bài toán này là áp dụng khai thác đặc trưng ảnh qua CNN và sử dụng RNN để sinh câu mô tả. Tuy nhiên, phần lớn các nghiên cứu hiện tại chủ yếu tạo chú thích bằng tiếng Anh hoặc tiếng Trung cho ảnh. Trong đồ án này, chúng tôi tập trung giải quyết bài toán Image Captioning cho tiếng Việt – ngôn ngữ đang có gần 100 triệu người sử dụng. Chúng tôi sẽ kế thừa bộ dữ liệu UIT-ViIC - bộ dữ liệu đầu tiên cho bài toán Image Captioning cho tiếng Việt và xây dựng mở rộng thêm bộ dataset này theo phương pháp được đề xuất trong bài báo nghiên cứu. Hướng tiếp cận của chúng tôi cho bài toán trên sẽ sử dụng EfficientNetV2 để trích xuất đặc trưng ảnh và Transformer cho việc hình thành câu mô tả. Chúng tôi hy vọng kết quả đạt được sẽ tạo động lực cho các nghiên cứu sâu hơn về lĩnh vực Image Captioning trên tiếng Việt cũng như đa ngôn ngữ.

   * **Input:** Một tấm ảnh có chứa môn thể thao có bóng.
   * **Output:** Câu mô tả bằng Tiếng Việt cho bức ảnh.
* **Các ngữ cảnh ứng dụng:** 
   -	*Hỗ trợ người khiếm thị:* Image Captioning có thể giúp người khiếm thị hiểu được nội dung của các hình ảnh mà họ không thể nhìn thấy. Bằng cách sử dụng các phần mềm đọc mô tả văn bản cho hình ảnh, người khiếm thị có thể sử dụng điện thoại thông minh hoặc máy tính để xem và hiểu được nội dung của các hình ảnh.
   -	*Mạng xã hội:* Image Captioning cũng được sử dụng để tạo ra mô tả cho các bức ảnh trên các mạng xã hội như Instagram, Facebook, Twitter, v.v. Điều này giúp cho người dùng có thể tìm kiếm và hiểu được nội dung của các bức ảnh một cách dễ dàng hơn.
   -	*Máy tính xử lý ảnh:* Image Captioning có thể được sử dụng trong các ứng dụng máy tính xử lý ảnh để giúp máy tính hiểu được nội dung của các hình ảnh. Các ứng dụng có thể bao gồm xác định đối tượng trong hình ảnh, phân loại hình ảnh, phát hiện hành động, v.v.
   -	*Giáo dục:* Image Captioning cũng có thể được sử dụng trong giáo dục để giúp học sinh và sinh viên hiểu được nội dung của các bức ảnh trong sách giáo khoa hoặc tài liệu học tập.
   -	*Các ứng dụng thương mại điện tử:* Image Captioning có thể được sử dụng trong các ứng dụng thương mại điện tử để giúp khách hàng hiểu được nội dung của các sản phẩm và đặt hàng một cách chính xác hơn.

## [MÔ TẢ BỘ DỮ LIỆU](#top)
* **Tên bộ dữ liệu:** UIT-ViIC + Flickr_sportballs
* **Thống kê:**
   * **UIT-ViIC** 
  
| **Dataset**              |  **Ảnh**                   |  **Caption**            |
| :----------------------: |:-------------------------: | :-----------------------:
|  **Train**               |  3619                      |  18101                  |
|  **Test**                |   231                      |  1155                   |

   * **Flickr_sportballs**
  
| **Dataset**              |  **Ảnh**                   |  **Caption**            |
| :----------------------: |:-------------------------: | :-----------------------:
|  **Train**               |  100                       |  500                    |
|  **Test**                |   100                      |  500                    |

* **Cách thức xây dựng:**

Bộ dữ liệu UIT-ViIC là bộ dữ liệu được các chuyên gia thu thập từ MS COCO và sử dụng các quy luật annotation để label caption Tiếng Việt cho các hình ảnh.

Bộ dữ liệu Flickr_sportballs là bộ dữ liệu do nhóm tự thu thập gồm 200 ảnh và 1000 câu mô tả (5 câu mô tả cho mỗi ảnh) dựa trên bộ dữ liệu Flickr30k. Công việc cần làm là mỗi thành viên của nhóm sẽ gán nhãn caption Tiếng Việt cho các hình ảnh môn thể thao có bóng trong bộ dữ liệu Flickr30k dựa trên một số quy luật annotation nhất định. Để tạo nên bộ dữ liệu Flickr_sportballs, nhóm tiến hành theo các bước sau đây:

   -  Bước 1: Lọc hình ảnh môn thể thao có bóng trong bộ dữ liệu Flickr30k
   
      Dựa vào bộ dữ liệu Flickr30k có caption Tiếng Anh cho trước. Nhóm tiến hành tìm kiếm những keyword được cho là có liên quan đến môn thể thao có bóng.
      Ví dụ: “bowling”, “tennis”, “baseball”, “basketball”, “football”,.....
      
   -  Bước 2: Làm sạch nhiễu
   
      Những hình ảnh có chứa keyword trên sẽ được chọn ra và tiến hành bước làm sạch nhiễu. Nhiễu ở đây được xem là những hình ảnh có chứa bóng nhưng không phải là một       hình ảnh mang tính thể thao hoặc những hình ảnh có chứa keyword ta cần nhưng không miêu tả một môn thể thao có bóng (“basketball basket”, “baseball cap”, …). 
      Ví dụ: “A man in a red apron wearing a baseball cap is sitting on a step.”
      
      Bước làm sạch nhiễu sẽ do các thành viên đánh giá khách quan hình ảnh đó có chứa nhiễu hay không.
      
   -  Bước 3: Xây dựng các quy định annotation
   
      Theo khảo sát một số caption của hình ảnh trên mạng bị đánh giá là không tốt do caption nó đưa ra không trùng khớp với những gì hình ảnh miêu tả như tên người,         tên địa điểm, thời gian, ... Bởi vì thế, để tạo ra những caption miêu tả đúng nghĩa chúng ta cần phải đặt ra những quy tắc chặt chẽ để tiến hành annotation. Dựa       trên những quy tắc có sẵn do các chuyên gia đề ra để annotation, chúng ta có các quy tắc như sau:
      
         -	Mỗi caption chứa ít nhất 6 từ tiếng Việt.
         -	Chỉ miêu tả những hoạt động và đối tượng hiện hữu trong bức ảnh.
         -	Không đề cập đến tên của các địa điểm, sự vật (tên thành phố, tên người, tên tòa nhà, ...) và các con số cụ thể (ngày giờ, số phòng,..)
         -	Các caption phải được viết bằng thì hiện tại tiếp diễn (continuous present tense).
         -	Những ý kiến và cảm xúc cá nhân không được bao gồm trong caption.
         -	Những đối tượng không rõ ràng (bị che khuất, không hoàn chỉnh, ...) sẽ bị bỏ qua.
         -	Đối với những đối tượng có cùng loại hay đặc điểm với số lượng nhiều, annotators không cần phải đề cập chúng trong caption.
      
      Sau khi xây dựng các quy tắc annotation các thành viên của nhóm sẽ tiến hành gán nhãn cho các hình ảnh trong bộ dữ liệu và kết hợp cùng sự giúp đỡ của các thành viên nhóm khác để tạo ra một bộ dữ liệu caption Tiếng Việt khách quan nhất.

## [MÔ TẢ THUẬT TOÁN](#top)

Xây dựng mô hình Image Captioning với phần encoder sẽ dựa trên *EfficientNetV2* (phương pháp do Mingxing Tan, Quoc V. Le công bố năm 2021) để trích xuất đặc trưng ảnh và phần decoder sẽ sử dụng *Transformer* (phương pháp do Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser, Illia Polosukhin công bố năm 2017) để sinh ra câu mô tả cho ảnh.

**Pipeline**

![image](https://github.com/leetnlok/CS114/blob/main/Final_Project/pipeline.png)

## [ĐÁNH GIÁ](#top)
* [BLEU](https://dl.acm.org/doi/10.3115/1073083.1073135)
* [ROUGE](https://aclanthology.org/W04-1013/)
* [CIDEr](https://arxiv.org/abs/1411.5726)

## [KẾT QUẢ](#top)
|  **Dataset**                         |  **BLEU-1**      |  **BLEU-2**      |  **BLEU-3**      |  **BLEU-4**      |  **ROUGE**   |  **CIDEr**    |
|  :--------------------------------:  |  :-------------: |  :-------------: |  :-------------: |  :-------------: |  :---------: |  :------------:
|  **UIT-ViIC**                        |  0.6965          |   0.5647         |  0.4671          |  0.395           |  0.5821      |  1.0668       |
|  **UIT – ViIC + Flickr_sportball**   |  0.6957          |   0.5562         |  0.4576          |  0.3863          |  0.5802      |  1.0703       |

* Mô hình: [colab](https://drive.google.com/file/d/193f3_fLwg-ya2XlnrqoV4_nBUwFq6XD2/view?usp=sharing)
* Báo cáo đồ án: [pdf](https://github.com/leetnlok/CS114/blob/main/Final_Project/report.pdf)
