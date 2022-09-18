# Snowboard

Khi dùng Exiftool , mục `Comment` mình thấy được flag : `CTFlearn{CTFIsEasy!!!}` nhưng mà khi nhập vào thì không được. 
Comment trên là comment đánh lừa, vì vậy mình nghĩ tới trường hợp còn comment khác, và với ảnh JPG/JPEG thì khá là dễ để tìm comment.

Vào hexeditor bất kì, tìm khối Hex `FF FE` rồi nhìn phần text đằng sau nó. Có thể thấy không chỉ có cái fake flag ở trên:


![Screenshot (2420)](https://user-images.githubusercontent.com/113530029/190896639-58a705bc-17be-4a69-a7b5-ec67f86a32f6.png)

Cái comment kế, nếu tiếp xúc đủ nhiều bạn có thể nhìn ra ngay nó được encode dùng base64.

Decode base64 bằng mấy tool online trên mạng, ta được Flag.
