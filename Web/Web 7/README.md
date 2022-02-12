Bài này giống như nhiều bài khác để lộ file robots.txt, sau khi truy cập ra nhận được path dẫn đến file **index.abc** 
![image](https://user-images.githubusercontent.com/62832067/153695869-c8f8b34a-bb30-45d5-802d-5ccfe857854c.png)
<br> Ở đây ta có 2 hàm cần chú ý là:
<br> Hàm ereg() check kí tự đặc biệt trong password, nếu password chứa kí tự đặc biệt sẽ có thông báo 
<br> ```if (ereg ("^[a-zA-Z0-9]+$", $_GET['password']) === FALSE)``` 
<br> Hàm in ra flag nếu giá trị ta nhập vào là **^_^** 
<br> ``` if (strpos ($_GET['password'], '^_^') !== FALSE)```
<br> ```        die('<h1><center>Flag: ' . $flag. '</center></h1>'); ```

