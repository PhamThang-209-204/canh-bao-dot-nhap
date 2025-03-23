ỨNG DỤNG CÔNG NGHỆ TRONG HỆ THỐNG CẢNH BÁO ĐỘT NHẬP
 


Made by AIoTLab Fit DNU DaiNam University

🌟 Giới thiệu
Hệ thống cảnh báo đột nhập sử dụng công nghệ nhận diện khuôn mặt và cơ sở dữ liệu db. Ứng dụng này cho phép người dùng dễ dàng bảo vệ an ninh của ngôi nhà, thực hiện nhận diện và báo động khi cần thiết.

🌟 Tính năng chính
Nhận diện tự động tự động: Hệ thống sử dụng camera để quét khuôn mặt người và phát âm thanh khi khuôn mặt được nhận diện. Hệ thống sẽ báo âm thanh chào mừng nếu là người quen ngược lại phát báo động.
Thông báo trực quan: Khi nhận dạng được người có trong dữ liệu, hệ thống sẽ hiển thị thông tin trên giao diện người dùng. Nếu có trường hợp không nhận diện được khuôn mặt sẽ = người lạ sẽ được hiển thị.
Quản lý dữ liệu: Dữ liệu nhận diện và thông tin người quen được lưu trữ trong SQL Server.
Giao diện thân thiện: Sử dụng Python tkinter cho giao diện người dùng với webcam để quét khuôn mặt, xử lý nhận dạng cũng như lưu dữ liệu. Giao diện người dùng được thiết kế đơn giản và dễ sử dụng.
Phát hiện khuôn mặt: Sử dụng thư viện BDPH để phát hiện khuôn mặt và cv2 để xác thực các khuôn mặt so với cơ sở dữ liệu đã lưu trữ.
Cải thiện hình ảnh: Hệ thống cải thiện chất lượng hình ảnh trước khi xác thực bằng các kỹ thuật như tăng độ nét và điều chỉnh độ sáng.
🏗️ HỆ THỐNG
System Architecture

📂 Cấu trúc dự án
BTL_IOT
├── 📂 data_face # File lưu ảnh nhận diện
│ ├── 🖼️ anh1.jpg # Ảnh tạm lưu trong quá trình nhận diện
│ ├── 🖼️ anh2.jpg # Ảnh tạm lưu trong quá trình nhận diện
├── 📂 intruders # File lưu ảnh người lạ
│ ├── 🖼️ anh1.jpg # Ảnh tạm lưu trong quá trình nhận diện
│ ├── 🖼️ anh2.jpg # Ảnh tạm lưu trong quá trình nhận diện
├── 📂 trainer # File trainner
│ ├── 📄 face-trainer.yaml # File trainer
├── 📄 _alert.mp3 # File âm thanh cảnh báo
├── 📄 _hello.mp3 # File âm thanh chào mừng
├── 📄 FaceBase.db # File dữ liệu database
├── 📄 giaodien.py # File code giao diện
├── 📄 KhuonMat.xml # File logic nhận diện
├── 📄 lay_dulieu.py # File code lấy dữ liệu
├── 📄 nhan_dien.py # File code nhận diện
├── 📄 training.py # File code training

🛠️ CÔNG NGHỆ SỬ DỤNG
📡 Phần cứng

CameraIP MTCNN DeepFace

Phần mềm
Python Flask OpenCV pyodbc [![React](https://img.shields.io/badge/React-17.0. ::contentReference[oaicite:0]{index=0}
Poster
![image](https://github.com/user-attachments/assets/78317cf0-d86b-45f3-a1e9-29de9b38dba5)
