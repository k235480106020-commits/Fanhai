# SQL SERVER 
**Họ & tên: Phan Văn Hải**  
**Lớp: K59.KMT.K01**  
**MSSV: K235480106020**  
---
1. Download và cài đặt SQL Server 2025
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/50732c1d-ee87-4496-8336-8c3f5405a177" />


2. Cấu hình cho SQL Server làm việc ở cổng động(Dynamic Port), TCP(36020):  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/20cca4ca-3db3-4028-96cd-65ebe9740cec" />


3. Kiểm tra xem Service SQL Server bằng Command Prompt
```powershell
netstat -ano | findstr LISTENING
```
<img width="960" height="539" alt="image" src="https://github.com/user-attachments/assets/6dde16b5-0497-4810-aa59-3a43cf5dcada" />


4. Cài Đặt SQL Server Management Studio
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6a3d0637-427d-47af-9773-655e26fb0dfe" />


5. Chạy phần mềm ssms để Đăng nhập vào SQL Server bằng 2 cách:


Windows Authentication
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/836b5fd3-6af5-4ed7-b3bd-d0dd90251913" />


SQL Server Authentication
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/77de4808-3df9-48dc-a6c5-35c1f936c9b4" />


6. File đã tạo ra database
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ddbb2fb7-e2f9-46b7-a8f6-8d859935c11f" />


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/525fb829-841a-4c82-9614-dbdec6756fe4" />


7. Tạo bảng dữ liệu và Primary Key(masv)  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/34971951-2f65-412a-a851-362f0fbacc13" />


 8. Import dữ liệu từ file csv mẫu vào bảng
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1c8799ba-cd02-4603-a18a-d56d3f88aca1" />


9. Kiểm tra xem số dòng của bảng sau khi import: 12020 dòng
```powershell
SELECT COUNT(*) AS SoDong FROM SinhVien;
```
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f6e1f715-d278-4f8f-900a-f0e7246226ae" />

10. Thêm 1 row vào bảng với dữ liệu là thông tin sinh viên
```powershell
INSERT INTO SinhVien (masv, hotensv, malop, ngaysinh, noisinh, diachi) 
VALUES ('K235480106020', N'Phan Văn Hải','K59KMT','26/01/2005', N'Vĩnh Phúc', N'Vĩnh Phúc');
SELECT * FROM SinhVien Where masv='K235480106020';
```
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b5f6e93c-b121-4cff-8318-4fe6cb6898a8" />


