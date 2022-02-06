Đầu tiên ta check signature ảnh thì đây đúng là file PNG
![image](https://user-images.githubusercontent.com/62832067/152694049-45a32337-e683-4df3-bccf-80b09a1fc89c.png)
<br> Bài này khó ko chịu được :). Ngồi mần thử các thể loại tool không được. Sau đấy tìm thử các cách sửa hex của file PNG. Theo kinh nghiệm thì ta có thể mần được một vài thông số có thể sửa như: hệ màu, chiều rộng, chiều cao
Theo như bài viết tra trên google thì ta có được các bytes tương ứng với width và height:
![image](https://user-images.githubusercontent.com/62832067/152694648-d40d16c3-1d64-4dc7-b533-ad9921541e5b.png)
![image](https://user-images.githubusercontent.com/62832067/152694635-dcd3eba4-b7f5-4774-a179-281b4c2c315e.png)

<br> Sau khi sửa height thành 700px (02 BC hệ hex) thì ta có được flag. Bên phải là ảnh gốc
![image](https://user-images.githubusercontent.com/62832067/152694050-fee6361a-ae59-4023-9107-1cb19dad18f1.png)
