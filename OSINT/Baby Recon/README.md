Bài gửi cho mình một hình ảnh favicon, ban đầu thì tưởng là soi ra đơn vị cung cấp của Viblo nhưng không phải, sau khi tra Google về "Favicon Osint" thì có 1 bài viết tham khảo về kĩ thuật Osint này:
[Link tham khảo](https://devansh.xyz/osint/2021/09/11/weaponizing-favicon-ico.html) 
<br> Y hệt như trong bài viết nói, mỗi một favicon được hash tương ứng với 1 IP và có 2 cách tính ra giá trị hash đó, 1 là dùng script Python trong bài viết, 2 là có 1 tool trên mạng như trong bài reddit này:
![image](https://user-images.githubusercontent.com/62832067/152735797-e8c08c77-043d-4718-9cca-da9093e163f7.png)
<br> Để lấy được url của favicon thì ta lên trang chủ Viblo CTF (vì file ta tải về là logo Viblo CTF)
<br> Ta thấy thẻ href như hình -> URL của favicon là https://ctf.viblo.asia/favicon.ico ![image](https://user-images.githubusercontent.com/62832067/152736011-e84f9546-1ff7-4019-8a4c-4d5bfaf0e13e.png)
<br> Ta có giá trị hash là: -1418078801
![image](https://user-images.githubusercontent.com/62832067/152736693-dbfa4938-7bc1-4a85-995e-b539519daf0d.png)
<br> Sau đó ta sử dụng Shodan với cú pháp: http.favicon.hash:[Favicon hash] để tìm được IP cùng đơn vị cung cấp hosting (tiên sư cái trang bắt login để search)
![image](https://user-images.githubusercontent.com/62832067/152737155-8b821e78-dbcc-4e5f-9a51-056f3ddfd9ae.png)
<br> Như kết quả ta có là Linode và server đặt ở Singapore -> Flag là: **Flag{Singapore_Linode}**
