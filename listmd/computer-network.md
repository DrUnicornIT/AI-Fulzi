---
layout: page
title: Computer NetWork
permalink: courseuet/computer-network
---
## Exam-Type-Option-Plus

## Exam
Câu 1. Trong các phát biểu sau phát biểu nào KHÔNG chính xác
- [x] Chồng giao thức của mạng Internet bắt buộc phải có 5 tầng: 1 tầng ứng dụng (application), 1 tầng giao vận (transport), 1 tầng mạng (network), 1 tầng liên kết dữ liệu (data link), và 1 tầng vật lý (physic)
- [ ] Mạng Internet bao gồm các mạng con kết nối với nhau, mỗi mạng có thể sử dụng các công nghệ hoàn toàn khác nhau ở tằng vật lý và tăng lên kết dữ liệu
- [ ] Chồng giao thức của mạng Internet có thể có tới 7 tầng.
- [ ] Mạng Internet bao gồm các mạng con kết nối với nhau, mỗi mạng có thể sử dụng các thuật toán tìm đường khác nhau.  

Giải thích
	Chồng giao thức của mạng Internet thực tế là mô hình OSI (Open Systems Interconnection) gồm 7 tầng, không phải 5 tầng. Các tầng trong mô hình OSI bao gồm: 1. Tầng vật lý (Physical Layer), 2. Tầng liên kết dữ liệu (Data Link Layer), 3. Tầng mạng (Network Layer), 4. Tầng giao vận (Transport Layer), 5. Tầng phiên (Session Layer), 6. Tầng trình diễn (Presentation Layer), và 7. Tầng ứng dụng (Application Layer).


Câu 2. Máy chủ Web proxy dùng cho các máy tính của một trường học cần đặt ở đâu để giảm tải cho đường truyền Internet của trường học đó?
- [ ] Ở vị trí bất kỳ trên mạng Internet 
- [ ] Trong mạng backbone của nhà cung cấp dịch vụ Internet (ISP) của trường học
- [x] Trong mạng nội bộ của trường học
- [ ] Gần máy chủ Web mà các máy tính của trường học đỏ truy cập nhiều nhất

Giải thích 
	+ sai. Giải thích: Web cache server (Máy chủ Web proxy) phải nằm trên tuyến đường từ một máy tính trong mạng của trường học đến một trong các web server được (NSD trong mạng trường học) truy cập, vì vậy “vị trí bất kỳ” là sai.
	+ sai. Giải thích: Mặc dù Web cache server có thể đặt ở trong mạng backbone của ISP, nhưng sẽ xa hơn so với đặt trong chính mạng của NSD (mạng trường học).
	+ đúng. Giải thích: Đây là nơi gần NSD nhất do đó có thể đạt hiệu quả cao nhất. 
	+ sai. Giải thích: Web cache server càng nằm xa mạng của NSD (mạng trường học) thì hiệu quả giảm tải trên đường truyền Internet càng giảm.

Câu 3. Trong kiến trúc giao thức TCP/IP, tầng IP cung cấp dịch vụ gì cho tầng giao vận?
- [ ] Truyền dữ liệu giữa các máy tính với độ trễ không đổi
- [ ] Đảm bảo các gói tin được truyền đến đúng tiến trình của bên nhận
- [x] Định tuyến gói tin đến đúng địa chỉ IP của bên nhận
- [ ] Đảm bảo truyền tin tin cậy giữa các máy tính có liên kết vật lý trực tiếp

Giải thích
	Trong kiến trúc giao thức TCP/IP, tầng IP (Internet Protocol) là tầng mạng và có trách nhiệm định tuyến gói tin từ nguồn đến đích trong mạng. Tầng IP xác định địa chỉ IP của các thiết bị mạng và sử dụng các giao thức định tuyến để định tuyến gói tin thông qua mạng từ một địa chỉ nguồn đến địa chỉ đích. Vì vậy, tầng IP cung cấp dịch vụ định tuyến gói tin đến đúng địa chỉ IP của bên nhận. Tầng giao vận (ví dụ: TCP hoặc UDP) sẽ đảm bảo truyền dữ liệu giữa các máy tính và đảm bảo các gói tin được truyền đến đúng tiến trình của bên nhận, nhưng các chức năng này không thuộc trách nhiệm của tầng IP.

Câu 4. Giao thức nào dùng để gửi email
- [ ] SSH
- [ ] DNS
- [ ] FTP
- [ ] IMAP
- [ ] HTTP
- [ ] POP3
- [x] SMTP

Giải thích
	Giao thức dùng để gửi email là SMTP (Simple Mail Transfer Protocol).

Câu 5. UDP được gọi là giao thức không hưởng kết nối (connectionless) vì
- [ ] Cả B và D
- [x] Tất cả gói tin UDP được đối xử một cách độc lập
- [ ] Tất cả các đáp án đều sai
- [ ] Nó gửi dữ liệu như là một luồng các gói tin liên quan đến nhau

Giải thích: 
	None

Câu 6. Dưới đây là bảng NAT translation table của một thiết bị NAT tại thời điểm hiện tại. Trong hai cột của bảng này, một cột là “Internet side” một cột là “Local side”. Nhìn vào nội dung của bảng, hãy ĐOÁN xem cột nào là Internet side, cột nào là Local side  
Cột 1  
136.4.6.7 : 210   
136.4.6.6 : 801  
1.2.3.4 : 986  
Cột 2  
192.168.10.44 : 4032  
192.168.6.4 : 1005  
192.168.5.4 : 1108  

1. Internet side 
- [ ] Cột 2
- [x] Cột 1
2. Local side 
- [x] Cột 2
- [ ] Cột 1

Giải thích: 
	Trong bảng NAT translation table, cột chứa địa chỉ IP và cổng trên mạng Internet được gọi là Internet side. Trong trường hợp này, cột 1 (136.4.6.7 : 210, 136.4.6.6 : 801, 1.2.3.4 : 986) chứa địa chỉ IP và cổng của các máy tính trên mạng Internet, vì vậy đó là Internet side.
	Cột chứa địa chỉ IP và cổng trên mạng nội bộ (Local Area Network) được gọi là Local side. Trong trường hợp này, cột 2 (192.168.10.44 : 4032, 192.168.6.4 : 1005, 192.168.5.4 : 1108) chứa địa chỉ IP và cổng của các máy tính trong mạng nội bộ, vì vậy đó là Local side.

Câu 7. Ứng dụng mạng (Network applications) có thể được xây dựng theo các kiến trúc nào sau đây?
- [ ] Peer-to-peer
- [ ] Client-Server
- [x] Cả B, A và D
- [ ] Hybrid

Giải thích:
	None

Câu 8.
Ghép kiểu gói tin được sử dụng bởi giao thức của các tầng tương ứng?

a. Tầng liên kết dữ liệu  i. Thông báo (messages)
b. Tầng mạn                   ii. Khung tin (frame)
c. Tầng giao vận            iii. Gói tin (packet)
d. Tầng ứng dụng          iv. Đoạn tin (segment)
- [x] a-ii b-iii c-iv d-i
- [ ] a-i b-li C-lii d-iv
- [ ] a-ii b-iv c-iii d-i
- [ ] a-li b-iv c-id-iii

Giải thích:
	Ghép kiểu gói tin được sử dụng bởi giao thức của các tầng tương ứng như sau:
	a. Tầng liên kết dữ liệu: ii. Khung tin (frame) 
	b. Tầng mạng: iii. Gói tin (packet) 
	c. Tầng giao vận: iv. Đoạn tin (segment) 
	d. Tầng ứng dụng: i. Thông báo (messages)

Câu 9. Mô hình OSI có bao nhiêu tầng
- [ ] 5
- [x] 7
- [ ] 4
- [ ] 10

Giải thích:
	Mô hình OSI (Open Systems Interconnection) có tổng cộng 7 tầng. Các tầng trong mô hình OSI bao gồm:
	1. Tầng vật lý (Physical Layer)
	2. Tầng liên kết dữ liệu (Data Link Layer)
	3. Tầng mạng (Network Layer)
	4. Tầng giao vận (Transport Layer)
	5. Tầng phiên (Session Layer)
	6. Tầng trình diễn (Presentation Layer)
	7. Tầng ứng dụng (Application Layer)

Câu 10. Để đảm bảo truyền dữ liệu tin cậy, TCP sử dụng cơ chế truyền lại
(retransmission). Cơ chế này được thực hiện khi nào ở bên gửi?
- [ ] Khi phát hiện lỗi checksum
- [x] Khi hết thời gian chờ nhận ACK (timeout)
- [ ] Khi phát hiện sai thứ tự gói tin
- [ ] Khi phát hiện trùng gói tin

Giải thích:
	Để đảm bảo truyền dữ liệu tin cậy, TCP sử dụng cơ chế truyền lại (retransmission). Cơ chế này được thực hiện khi bên gửi không nhận được ACK (acknowledgment) từ bên nhận trong khoảng thời gian chờ nhận ACK (timeout). Khi thời gian chờ đã hết mà không nhận được ACK, TCP sẽ cho là gói tin đã bị mất trong quá trình truyền và sẽ gửi lại gói tin đó. Việc truyền lại gói tin nhằm đảm bảo rằng dữ liệu được nhận đúng và đầy đủ tại bên nhận. Cơ chế này giúp TCP xử lý các vấn đề như mất gói tin trong quá trình truyền hoặc thời gian chờ quá lâu mà không nhận được phản hồi từ bên nhận.

Câu 11. Các phát biểu dưới đây đúng hay sai ?
- [ ] Chỉ cần SMTP là đủ cho các hệ thống email phổ biến hiện nay hoạt động được
- [x] Thông tin điều khiển và dữ liệu tải file của FTP được chạy trên cùng một kết nối
TCP
- [ ] HTTP request và HTTP response chạy trên hai kết nối TCP khác nhau
- [x] Mỗi một HTTP request tương ứng với một hoặc nhiều HTTP response
- [x] Mỗi một chu kỳ Request-response của HTTP chỉ có thể chạy trên cùng 1 kết nối
TCP
- [x] HTTP protocol chỉ có hai loại bản tin là HTTP request và HTTP response
- [x] HTTP có thể được sử dụng để truyền file giống như FTP
- [x] FTP chạy trên port 20
- [x] FTP chạy trên port 21
- [x] HTTP chạy bên trên TCP protocol

Câu 12. Chọn kết luận sát thực tế nhất về “Độ dài lớn nhất của một frame trong
chuẩn 802.3 (Ethernet)” là
- [x] 1518
- [ ] 1230
- [ ] 1021
- [ ] 2048

Câu 13. Địa chỉ IP 127.0.0.1 là:
- [ ] địa chỉ quảng bá lớp A
- [ ] địa chỉ broadcast
- [ ] địa chỉ multicast
- [x] địa chỉ loopback

Câu 14. Trong các tài liệu về mạng máy tính hiện nay, các tác giả hay sử dụng các
ví dụ dựa trên mạng Internet để có tính thực tế. Đề có tính lý thuyết cao, họ cũng
thường sử dụng mô hình ... (có 7 tầng) để trình bày  
Ans: _OSI_

Câu 15. Giao thức nào được sử dụng để cấu hình địa chỉ IP cho client (IP address,
netmask, default gateway, DNS server)?
- [ ] SNMP
- [ ] ARP
- [ ] SMTP
- [x] DHCP

Câu 16. Dịch vụ thư điện tử sử dụng giao thức nào ở tầng ứng dụng
- [ ] HTTP
- [ ] SIP
- [ ] FTP
- [x] SMTP

Câu 17. Chọn "Đúng" hoặc "Sai" cho các ý sau về chức năng của router
- [ ] Ngăn xung đột
- [x] Lựa chọn tuyến đường
- [x] Chuyển tiếp các gói tin
- [x] Lọc bỏ các gói tin

Câu 18. Lựa chọn các chức năng của switch
- [ ] đánh địa chỉ IP
- [x] tránh các vòng lặp
- [x] forwarding và lọc frame theo MAC
- [x] học địa chỉ MAC
- [ ] định tuyến

Câu 19. Trong biểu diễn nhị phân, đâu là phạm vi của lớp địa chỉ (class) B
- [ ] 111...
- [ ] 110...
- [x] 10...
- [ ] 01...
- [ ] 0...

Câu 20. Giao thức TCP là một giao thức
- [ ] Hướng kết nối (connection oriented)
- [ ] Sử dụng quy trình bắt tay ba bước để khởi tạo kết nối
- [x] Cả 3 đáp án đều đúng
- [ ] Gom dữ liệu từ các ứng dụng thành một luồng duy nhất

Câu 21. Hai máy tính A (IP: 10.10.0.1/24) và B (IP: 172.16.0.1/24) có thể trao đổi dữ
liệu với nhau bình thường, Khi tầng Application từ A cần gửi thông tin đến tầng
Application của B, bên trong khung tin (frame) đi ra từ tầng liên kết dữ liệu (data link)
của máy A gửi đến máy B sẽ chứa
- [ ] MAC của A, MAC của B, IP của A, IP của B
- [ ] MAC của A, IP của A, IP của B
- [ ] MAC của B, IP của A, IP của B
- [x] MAC của A, MAC của B.

Câu 22. Dịch vụ DNS có thể cân bằng tải cho các Web server được nhân bản của
cùng một trang Web bằng cách nào?
- [ ] Gán nhiều biệt danh (alias name) cho tên miền của trang Web, mỗi biệt danh
ứng với một Web server
- [x] Lưu tập địa chỉ IP của các Web server trong bản ghi DNS ứng với tên miền của
trang Web
- [ ] DNS server chuyển các thông báo HTTP request đến các Web server một cách
ngẫu nhiên
- [ ] Đăng ký tên miền của trang Web với nhiều authoritative DNS server

Câu 23. Trong một mạng LAN có cài đặt một router có chức năng DHCP và DNS.
Trễ đầu cuối đến đầu cuối (end-to-end) giữa hai máy bất kỳ trong LAN giả định là
30ms (không đổi, không phụ thuộc kích thước gói tin, không phụ thuộc vào tính toán
tại mỗi nút). Một máy tính (máy C) được cấu hình sử dụng DHCP được bật lên và
cắm vào mạng LAN đó. Ngay sau khi máy C được cấp phát thành công một địa chỉ
IP, C thực hiện một câu truy vấn tên miền www.vnexpress.net đến máy chủ DNS nội
bộ của mạng LAN. Giả sử rằng tên miền www.vnexpress.net đã được cache tại máy
chủ DNS nội bộ. Hỏi: Sau bao nhiêu ms kể từ lúc máy C gửi truy vấn tên miền, máy
tính C sẽ nhận được phản hồi cho câu truy vấn tên miền www.vnexpress.net. (Chỉ
điền giá trị số)  
Ans: _60_

Câu 24. Cho đoạn dữ liệu gồm 5 byt- [ ] Mỗi byte được biểu diễn dưới dạng mã hexa
như bảng dưới. Tính Internet checksum của đoạn dữ liệu đó. Yêu cầu viết kết quả
dưới dạng hexa (không điền tiền tố Ox). Ví dụ 1F3E

|Byte thứ   | 1 | 2   | 3   |   4 |   5 |
|-| - | -   | -   |   - |   - |
|Giá trị      |12 | 00 | 01 | 00 | A0 |

Ans: _4CFF_

Câu 25. Câu nào diễn đạt đúng về switch?
- [ ] tạo ra nhiều miền collision và nhiều miền broadcast
- [ ] tạo ra một miền collision và nhiều miền broadcast
- [x] tạo ra nhiều miền collision và một miền broadcast
- [ ] tạo ra một miền collision và một miền broadcast

Câu 26. Trong các giao thức sau, giao thức nào chạy ở tầng ứng dụng và không sử
dụng TCP để truyền/nhận dữ liệu
- [x] DNS
- [ ] ARP
- [ ] IP
- [ ] HTTP

Câu 27. Câu nói nào là đúng?
- [x] Các máy tính đầu cuối luôn có subnet mask
- [ ] Subnet mask được gán cho các thiết bị ở lớp địa chỉ (class) - [ ]
- [ ] Các thiết bị được gán cho một subnet mask chỉ khi chúng thuộc về cùng một
mạng con
- [ ] Subnet mask chỉ được sử dụng ở lớp địa chỉ (class) A và B

Câu 28. Các chức năng của link layer được thực hiện ở đâu trong host
- [x] Network interface card (card mạng) và hệ điều hành
- [ ] Hệ điều hành
- [ ] Bộ nhớ
- [ ] Network interface card (card mạng)

Câu 29. NAT giữa một mạng local và mạng Internet làm việc như thế nào
- [ ] Dịch địa chỉ IP sang địa chỉ MAC
- [ ] Dich Hostname sang IP
- [x] Dịch địa chỉ IP công cộng (public IP) sang địa chỉ IP riêng (private IP) và ngược
lại
- [ ] Không đáp án nào đúng

Câu 30. Độ lớn của trường checksum trong gói tin TCP là bao nhiêu bit
- [x] 16
- [ ] 64
- [ ] 32
- [ ] 0

Câu 31. Trong giao thức TCP, bên gửi nhận biết sự tắc nghẽn của mạng bằng cách
nào?
- [ ] Router bị tắc nghẽn sẽ đánh dấu vào gói tin để bên nhận biết có sự tắc nghẽn và
gửi thông tin này cho bên nhận
- [ ] Bên nhận dựa vào độ trễ của gói tin biên nhận ACK để biết có tắc nghẽn hay
không
- [x] Khi hết thời gian timeout mà không nhận được gói tin biên nhận ACK hoặc nhận
được 3 gói tin ACK trùng lặp
- [ ] Router bị tắc nghẽn sẽ gửi thông báo cho bên gửi

Câu 32. Bộ định tuyến CIDR nhận được gói tin với địa chỉ đích là 131.23.151.76.
Bảng định tuyến của nó có các mục sau:

|Prefix         |Output Interface Identifier|
| --------------| ---------------------------|
| 131.16.0.0/12 |  3|
| 131.28.0.0/14 |  5|
| 131.19.0.0/16 |  2|
| 131.22.0.0/15 |  1|

Định danh của giao diện mà gói tin sẽ được chuyển tiếp là ?
- [ ] 2
- [ ] 5
- [x] 1
- [ ] 3

Câu 33. Các phát biểu dưới đây đúng hay sai ?
- [x] Mạng Internet nghẽn chủ yếu ở mạng lõi (Core network)
- [ ] Mạng Internet có thể đảm bảo dữ liệu được truyền đến đích theo thời gian thực
- [x] Asynchronous Data Subscriber Line (ADSL) là một công nghệ mạng truy nhập
- [ ] Mạng Internet là một mạng đơn giản với các đầu cuối thông minh
- [x] Đóng gói dữ liệu (encapsulation) nghĩa là bọc gói dữ liệu của tầng dưới vào trong
gói dữ liệu của tầng trên
- [ ] Do mạng Internet được thiết kế với các yêu cầu đơn giản nên nó có thể có quy mô
rất lớn.
- [x] Mạng Internet có thể đảm bảo dữ liệu truyền là tin cậy

Câu 34. DHCP cung cấp gì cho client
- [ ] Không đáp án nào đúng
- [x] Địa chỉ IP
- [ ] Địa chỉ MAC
- [ ] URL

Câu 35. Trong bản ghi tài nguyên của DNS, trường TTL (Time to live) được lưu trữ
trong 31 bit:
Hỏi: Thời gian sống tối đa của bản ghi tài nguyên DNS có thể được thiết lập vào
khoảng?
- [ ] 65 năm
- [ ] 67 năm
- [ ] 66 năm
- [x] 68 năm

Câu 36. Bảng dưới là 8 byte dữ liệu được thêm các bit chẵn lẻ 2 chiều. Cột 1 đến 8
và hàng 1 đến 8 là các bit dữ liệu. Cột 9 và hàng 9 là các bit chẵn lẻ cho hàng và
cột.
Trong tổng số các bit chỉ có 1 bit sai nằm ở phần dữ liệu (hàng 1 đến 8, Cột 1 đến
8). Tìm bit đó (viết kết quả một cách CHÍNH XÁC theo định dạng (hàng,cột) ví dụ
(6,7))

| | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | P |
|-|-|-|-|-|-|-|-|-|-|
|1 |0 |0 |1 |1 |0 |0 |1 |0 |1 |
|2 |1 |1 |0 |0 |0 |1 |1 |0 |0 |
|3 |1 |1 |0 |0 |0 |1 |1 |1 |0 |
|4 |1 |1 |0 |1 |1 |0 |0 |1 |1 |
|5 |0 |0 |0 |1 |0 |0 |1 |1 |1 |
|6 |1 |1 |1 |0 |1 |1 |0 |0 |1 |
|7 |0 |0 |0 |0 |0 |0 |0 |0 |0 |
|8 |0 |1 |1 |0 |0 |0 |0 |0 |0 |
|P |0 |0 |1 |1 |0 |1 |0 |1 |0 |

Ans: _(3,2)_

Câu 37. Tham số nào sau đây quyết định khả năng định tuyến (số gói tin định
tuyến/1s) của một router?
- [ ] Độ lớn của bộ nhớ ở cổng vào (input port)
- [x] Tốc độ xử lý của switching fabric
- [ ] Độ lớn của bộ nhớ ở cổng ra (output port)
- [ ] Số lượng công vào (input port) và cổng ra (output port)

Câu 38. Bob truy nhập vào trang www.vnexpress.net sử dụng HTTP 1.1. Trang chủ
vnexpress.net chứa 15 hình ảnh. Số lượng kết nối TCP được thực hiện là?
- [ ] 2
- [ ] 15
- [ ] 16
- [x] 1

Câu 39. Giao thức nào biết được địa chỉ MAC của một nút mạng, sau đó tạo ra cơ
sở dữ liệu lưu tạm thời ánh xạ địa chỉ IP - địa chỉ MAC
- [ ] DNS
- [ ] IP
- [x] ARP
- [ ] RARP
- [ ] UDP

Câu 40.
Giả thiết rằng:
- Khi một máy gửi một file F cho máy khác thì thời gian gửi luôn cố định bằng 1 giây
- Một máy chỉ gửi được file cho 1 máy khác tại cùng một thời điểm
Nếu có một server chia sẻ file F đó cho N máy khách theo kiểu client-server, sau 3
giây, Có thể có tối đa bao nhiêu máy sẽ có file F (tính bao gồm cả server)? (Chỉ điền
số vào ô nhập kết quả)  
Ans: _4_

Câu 41. Trong quá trình truyền tin từ máy A sang máy B, gói tin lần lượt đi qua 3 môi
trường có MTU khác nhau lần lượt là 4980, 1500, 2500 bytes. Hãy cho biết khi gửi
7500 byte dữ liệu từ A đến B thì bên B nhận được bao nhiêu gói tin trước khi ghép
mảnh?
- [ ] 3
- [x] 6
- [ ] 11
- [ ] 27

Câu 42. Trong thuật toán định tuyến nào tất cả các router có thông tin đầu vào giống
nhau
- [ ] Link Vector
- [x] Link State
- [ ] Distance Vector
- [ ] Shortest path

Câu 43. Tầng giao vận (transport layer) gom dữ liệu từ các ứng dụng khác nhau
thành một luồng duy nhất trước khi chuyển xuống cho
- [ ] Tầng ứng dụng (application layer)
- [ ] Tầng liên kết (data link layer)
- [ ] Tầng vật lý
- [x] Tầng mạng (network layer)

Câu 44. Mạng ở hình dưới hoạt động theo kiểu chuyển mạch gói (packet switching).
Cho biết các dữ kiện sau:
- Trễ lan truyền (propagation delay) bằng 1 ms với mọi link
- Kích thước các gói tin là 1000 bit
- Tốc độ truyền (transmission rate) trên mỗi link là như nhau và bằng 1000 bps
- Mạng không nghẽn (trễ hàng đợi, queueing delay) tại các nút bằng 0
Hỏi: Trễ truyền 1 gói tin từ S đến R là bao nhiêu ms ? (điền kết quả là một số với giá
trị là thời gian trễ với đơn vị milisecond. Ví dụ: 10)
S ---------- N1 ---------- N2 ---------- R    
Ans: _3003_

Câu 45. Chọn "Đúng" hoặc "Sai" cho các ý dưới đây về khái niệm Lõi mạng
(network core) trong mạng Internet. (Gợi ý: có 2 ý đúng)
- [x] Vận chuyển gói tin theo cơ chế chuyển mạch gói (packet switch)
- [ ] Là một mạng lưới các thiết bị switch kết nối với nhau
- [ ] Bao gồm các client và server
- [x] Là một mạng lưới các thiết bị router kết nối với nhau
- [ ] Vận chuyển gói tin theo cơ chế chuyển mạch điện (circuit switch)

Câu 46. Theo mô hình OSI, router thuộc về tầng nào:
- [ ] tầng session
- [ ] tầng physical
- [ ] tầng data link
- [x] tầng network

Câu 47. Địa chỉ IP của máy tính A là 110.2.112.12/20, địa chỉ IP của máy tính X là
110.2.109.4/20 và địa chỉ IP của máy tính Y là 110.2.105.20/20. Những máy tính nào
có cùng địa chỉ mạng (subnet)?
- [x] Máy tính X và máy tính Y
- [ ] Cả 3 máy tính
- [ ] Máy tính A và máy tính Y
- [ ] Máy tính X và máy tính A

Câu 48. Trong giao thức CSMA/CD, nếu 2 máy tính cùng đồng thời truyền 2 khung
tin vào môi trường truyền thì 2 máy tính này sẽ
- [ ] Gửi cảnh báo xung đột cho nhau và tiếp tục truyền
- [ ] Chỉ phát hiện được xung đột sau khi nhận được gói tin biên nhận ACK
- [x] Phát hiện được xung đột và ngừng truyền dữ liệu ngay lập tức
- [ ] Tăng mức năng lượng của tín hiệu truyền để giảm nguy cơ bị lỗi do xung đột xảy
ra

Câu 49. Khi một gói tin rời khỏi mạng, Router NAT thay thế địa chỉ nguồn của gói tin
đó bằng
- [ ] Địa chỉ IP đích
- [x] Địa chỉ IP của NAT router
- [ ] Địa chỉ port đích
- [ ] Không đáp án nào đúng

Câu 50. Card mạng Ethernet làm gì khi xảy ra xung đột
- [ ] Tiếp tục truyền
- [ ] Đợi 10 phút rồi truyền lại từ đầu
- [ ] Đợi 2 phút rồi truyền tiếp
- [x] Dừng truyền ngay lập tức

Câu 51. Loại địa chỉ nào trên máy tính đầu cuối mà ứng dụng sử dụng để có thể
nhận được dữ liệu từ nơi khác chuyển tới
- [ ] IP address
- [ ] MAC address
- [x] Port address
- [ ] NIC address

Câu 52. Máy tính A gửi cho máy tính B gói tin TCP thứ nhất có số thứ tự (sequence
number) là 2000 và độ dài gói tin là 1000 byte, và gửi gói tin TCP thứ hai có số thứ
tự là 3000 và độ dài gói tin là 200 byt- [ ] Tuy nhiên, máy tính B chỉ nhận được gói tin
TCP thứ hai. Hỏi sau khi nhận gói tin TCP thứ hai, máy tính B gửi gói tin biên nhận
ACK cho máy tính A với ACK bằng bao nhiêu?
- [ ] 1000
- [ ] 3200
- [x] 2000
- [ ] 3000

Câu 53. Bảng định tuyến của router A có các dòng được liệt kê như bên dưới, hãy
cho biết nếu một gói tin có địa chỉ đích là 203.113.119.1 thì dòng nào sẽ được chọn
để định tuyến cho gói tin đó
- [ ] Destination 203.113.192.0/18 → Gateway 200.176.10.1
- [x] Destination 203.113.64.0/18 → Gateway 113.57.10.1
- [ ] Destination 203.113.128.0/17 → Gateway 14.8.10.1
- [ ] Destination 203.113.0.0/16 → Gateway 193.168.10.1

Câu 54. Giao thức UDP thường được dùng với ứng dụng nào sau đây?
- [x] Ứng dụng nói chuyện trực tuyến (voice chat)
- [ ] Ứng dụng Web
- [ ] Ứng dụng truyền file
- [ ] Ứng dụng thư điện tử

Câu 56. Điều nào sau đây đúng với giao thức định tuyến theo thuật toán distance
vector ?
- [ ] Các bộ định tuyến không trao đổi thông tin với nhau
- [x] Các bộ định tuyến trao đổi distance vector với các nút lân cận (neighbour node)
- [ ] Các bộ định tuyến trao đổi bảng định tuyến với nhau
- [ ] Các bộ định tuyến sử dụng bảng định tuyến tính

Câu 57. Trong giao thức Go-Back-N có độ lớn cửa sổ là 6, A cần gửi các gói có số
thứ tự từ 0 đến 6 tới - [ ] Gói 3 trên đường đến B bị lỗi nên không đến được, phải gửi
lại 1 lần. Tính số gói (kể cả ACK từ B) mà A và B đã gửi cho nhau sau khi quá trình
gửi kết thúc.  
Ans: _21_

Câu 58. Dịch vụ nào chuyển đổi tên miền và hostname sang địa chỉ IP
- [ ] Network Time Protocol (NTP)
- [ ] Internet Relay Chat (IRC)
- [ ] Routing Information Protocol (RIP)
- [x] Domain Name System (DNS)

Câu 59. Được biết ngưỡng (threshold) hiện tại của quá trình kiểm soát tắc nghẽn là
16, hãy xác định giá trị của cửa sổ chống tắc nghẽn (congwin) khi bên gửi đã gửi
tổng số 35 segment và nhận đầy đủ số ACK trả về mà không có bất kỳ lỗi nào
- [ ] 17
- [ ] 18
- [x] 16
- [ ] 19

Câu 60. Một mạng LAN hình trạng bus có chiều dài 2km. Tốc độ lan truyền tín hiệu trên dây là 2 x 10^8 m/s. Mạng sử dụng CSMA/CD để truy nhập đường truyền và có tốc độ truyền dữ liệu là 10^7 bps . Trong CSMA/CD, người ta sử dụng cơ chế nghe đường truyền để phát hiện đụng độ (collision detection) trong khi vẫn đang truyền tin. Để máy phát hiện đụng độ trong khi truyền, thì tín hiệu sau khi đụng độ lại tiếp tục được truyền đi tiếp rồi quay lại máy đang truyền trong khoảng thời gian máy đang truyền tin. Trường hợp xấu nhất đề máy truyền tín hiệu và tín hiệu lại quay trở về máy là hai lần khoảng thời gian lan truyền tín hiệu trong mạng. Khoảng thời gian này tương đương với việc máy truyền từ bit đầu tiên đến bit cuối cùng của khung tin. Như vậy, để đảm bảo mọi đụng độ đều có thể được phát hiện trong khi máy đang truyền tin thì kích cỡ nhỏ nhất của khung tin được sử dụng trong mạng LAN này nên là ?
- [ ] 100 bytes
- [x] 25 bytes
- [ ] 200 bytes
- [ ] 50 bytes

Câu 61. Hub là thiết bị truyền tin?
- [ ] Cả ba lựa chọn kia
- [x] Quảng bá
- [ ] Điểm tới điểm
- [ ] Đa điểm.

Câu 62. Máy tính A gửi 1 gói tin IP cho máy tính B không nằm cùng một subnet. Hỏi
khung tin (frame) của layer 2 chứa gói tin IP khi gửi đi sẽ có địa chỉ MAC đích là địa
chỉ nào?
- [x] Địa chỉ MAC của router
- [ ] Địa chỉ MAC của máy tính A
- [ ] Địa chỉ MAC FFFFFFFFFFF
- [ ] Địa chỉ MAC của máy tính B

Câu 63. Máy tính của Ngân có IP là 17.84.129.73/19, hãy viết địa chỉ Broadcast của
mạng IP mà máy tính của Ngân đang tham gia dưới dạng a.b.c.d/x.y.z.t  
Ans: _17.84.157.255/255.255.224.0_

Câu 64. Cơ chế phân cấp nào hỗ trợ ánh xạ tên máy tính (hostname) và địa chỉ IP:
- [ ] RARP
- [ ] ARP
- [ ] LDAP
- [ ] IP
- [x] DNS

Câu 65. Nếu người ta dùng 10 bit để biểu diễn một ký tự và tốc độ đường truyền là
1200bps thì bao nhiêu kí tự sẽ được truyền trong một giây?
- [ ] 12
- [x] 120
- [ ] 1200
- [ ] 10

Câu 66. Chồng giao thức của mạng Internet có hình gì?
- [ ] Hình thang
- [ ] Hình kim tự tháp
- [x] Hình đồng hồ cát
- [ ] Hình chữ nhật

Câu 67. Router A chỉ có 2 node hàng xóm là router B và router C, với chi phí của kết
nối từ A đến B và C lần lượt là 2 và 5, B gửi cho A bảng distance vector của mình,
trong đó khoảng cách ngắn nhất đến node X từ B được thiết lập là 5. C gửi cho A
bảng distance vector của mình, trong đó khoảng cách ngắn nhất đến node X từ C
được thiết lập là 3. Hỏi router A sẽ ước lượng khoảng cách ngắn nhất từ A đến X
bằng bao nhiêu?
- [ ] 8
- [ ] 5
- [x] 7
- [ ] 2

Câu 68. Mạng ở hình dưới hoạt động theo kiểu chuyển mạch kênh (circuit
switching). Cho biết các dữ kiện sau:
- Trễ lan truyền (propagation delay) bằng 1 ms với mọi link
- Kích thước các gói tin là 1000 bit
- Tốc độ truyền (transmission rate) trên mỗi link là như nhau và bằng 1000 bps
- Mạng không nghẽn (trễ hàng đợi, queueing delay) tại các nút bằng 0.
Hỏi: Trễ truyền 1 gói tin từ S đến R là bao nhiêu ms ? (điền kết quả là một số với giá
trị là thời gian trễ với đơn vị milisecon- [ ] Ví dụ: 10)
S ---------- N1 ---------- N2 ---------- R  
Ans: _1003_

Câu 69. Topo mạng nào gồm 1 cáp mạng nối tất cả các nút trên mạng
- [x] Bus
- [ ] Ring
- [ ] Star
- [ ] ring-star

Câu 70. Các câu trả lời dưới đây là "Đúng" hay "Sai" đối với câu hỏi "Giao thức
mạng quy định gì ?" (network protocol)
- [x] Hành vi sẽ thực hiện khi nhận được bản tin
- [x] Format của bản tin (message) gửi và nhận
- [ ] Port number của ứng dụng
- [x] Kích cỡ của bản tin
- [x] Thứ tự gửi và nhận bản tin

Câu 71. Trong thuật toán định tuyến distance vector, mỗi node trao đổi distance
vector của nó với
- [ ] Các node hàng xóm và các node lân cận node hàng xóm
- [ ] Không trao đổi với ai
- [x] Các node hàng xóm
- [ ] Toàn bộ node trên mạng

Câu 72. Giao thức DHCP cung cấp cho client
- [ ] Địa chỉ IP khi client kết nối vào mạng
- [x] Tất cả đáp án đều đúng
- [ ] Tên và địa chỉ IP của DNS Server
- [ ] Địa chỉ IP của router đầu tiên trong mạng (first hop router)

Câu 73. Alice truy nhập vào trang thương mại điện tử alibabe.cn để mua hàng trực tuyến bằng trình duyệt Chrome. Điều nào sau đây KHÔNG đúng về khái niệm cookie?
- [x] Cookie có độ dài cố định
- [ ] Cookie là đoạn dữ liệu về người dùng
- [ ] Cookie được tạo ra bởi máy chủ (cụ thể alibae.cn)
- [ ] Cookie cho phép người dùng xem được lịch sử đến một website

Câu 74. Tầng giao vận xử lý vấn đề
- [ ] Tất cả lựa chọn đều sai
- [ ] Trao đổi thông tin giữa các node
- [x] Trao đổi thông tin giữa các tiến trình (process)
- [ ] Trao đổi thông tin giữa các ứng dụng

Câu 75. Các diễn đạt dưới đây về một địa chỉ Ethernet lớp 2 là "Đúng" hay "Sai"
- [x] Được gọi là địa chỉ vật lý
- [ ] Địa chỉ này sẽ thay đổi khi thiết bị di chuyển từ subnet này sang subnet khác
- [ ] Địa chỉ được thể hiện bởi 4 khối, mỗi khối là một chuỗi 12 bit nhị phân
- [x] Có chiều dài 48 bit

Câu 76. Đánh dấu "Đúng" hoặc "Sai" cho các ý sau khi một máy tính A di chuyển từ
subnet này sang subnet khác
- [ ] Địa chỉ default gateway lưu trên máy A phải giữ nguyên
- [x] Máy A vẫn hoạt động với địa chỉ MAC cũ
- [ ] Các ứng dụng chạy trên máy A cần phải được gắn thêm địa chỉ port
- [x] Địa chỉ IP của máy A phải được gán lại
- [ ] Địa chỉ MAC của máy A phải được gán lại

Câu 77. Một con số 32 bit, được sử dụng cùng địa chỉ IP của thiết bị để xác định địa
chỉ mạng (subnet) của thiết bị là.
- [ ] ARP address
- [ ] MAC address
- [ ] DNS mask
- [x] subnet mask

Câu 78. Trong mạng cục bộ Ethernet, điều nào sau đây là đúng?
- [ ] Tín hiệu đụng độ được dùng để bổ trợ cho các khung tin với kích cỡ nhỏ
- [x] Thời gian chờ thay đổi theo thuật toán exponential backoff làm giảm xác suất
đụng độ khi truyền lại
- [ ] Bên gửi dừng nghe đường truyền khi bắt đầu gửi khung tin
- [ ] Bên gửi vẫn tiếp tục gửi khung tin sau khi nghe được đụng độ

Câu 79. Câu nào diễn đạt đúng về giao thức IP?
- [ ] IP là giao thức tin cậy
- [ ] IP là giao thức hướng nối (connection oriented)
- [ ] IP là giao thức đảm bảo thời gian thực
- [x] IP là giao thức không hướng nối (connectionless oriented)

Câu 80. Cho 2 byte dữ liệu dưới dạng mã hexa A0B1. Tính 3-bit CRC của 2 byte dữ
liệu đó biết rằng CRC generator G dưới dạng nhị phân là 1001.  
Ans: _110_

Câu 81. Khi Bob gửi e-mail cho Alice, máy tính của Alice không kết nối mạn- [ ] Khi
đó, email của Bob sẽ nằm ở đâu?
- [x] Trong mail box của Alice trên mail server của Alice
- [ ] Trong hàng thư chờ gửi trên mail server của Bob
- [ ] Trong hàng thư chờ gửi trên mail server của Alice
- [ ] Trong mail box của Bob trên mail server của Bob

Câu 82. Thiết bị kết nối mạng nào cho phép nhiều nút đồng thời cũng gửi và nhận
trên các segment mạng khác nhau
- [ ] Hub
- [x] Switch
- [ ] Amplifier
- [ ] Repeater

Câu 83 - 84: Một gói tin có kích thước 2000 bytes được truyền giữa hai máy tính
trong mạng LAN. Biết khoảng cách vật lý giữa 2 máy tính là 400m, băng thông trong
mạng LAN là 100 Mbps. Biết vận tốc lan. truyền tín hiệu trong mạng LAN là 2x10^8
m/s.

Câu 83. Thời gian truyền dữ liệu (transmission time) vào mạng LAN là bao nhiêu?
- [ ] 0.00001 s
- [x] 0.00016 s
- [ ] 0.00002 s
- [ ] 0.00008 s

Câu 84. Thời gian lan truyền (propagation time) của gói tin giữa hai máy tính là bao
nhiêu?
- [ ] 0.00004 s
- [ ] 0.000016 s
- [x] 0.000002 s
- [ ] 0.00001 s

Câu 85. Loại địa chỉ nào trên máy tính đầu cuối mà ứng dụng sử dụng để có thể nhận
được dữ liệu từ nơi khác chuyển tới
- [ ] IP address
- [x] MAC address
- [ ] NIC address
- [x] Port address

Câu 86. Cho 2 byte dữ liệu dưới dạng mã hexa A0B1. Tính 3-bit CRC của 2 byte dữ
liệu đó biết rằng CRC generator G dưới dạng nhị phân là 1001.  
Ans: _110_

Câu 87. Hub là thiết bị truyền tin?
- [ ] Điểm tới điểm
- [ ] Đa điểm
- [ ] Cả ba lựa chọn kia
- [x] Quảng bá

Câu 88. Câu nào diễn đạt đúng về switch?
- [x] tạo ra nhiều miền collision và một miền broadcast
- [ ] tạo ra nhiều miền collision và nhiều miền broadcast
- [ ] tạo ra một miền collision và nhiều miền broadcast
- [ ] tạo ra môṭmiền collision và môṭmiền broadcast

Câu 89. Câu nói nào là đúng?
- [ ] Subnet mask chỉ được sử dụng ở lớp địa chỉ (class) A và B
- [x] Các máy tính đầu cuối luôn có subnet mask
- [ ] Subnet mask được gán cho các thiết bị ở lớp địa chỉ (class) A
- [ ] Các thiết bị được gán cho một subnet mask chỉ khi chúng thuộc về cùng một mạng con

Câu 90. Câu nào diễn đạt đúng về giao thức IP?
- [ ] IP là giao thức đảm bảo thời gian thực
- [ ] IP là giao thức tin cậy
- [ ] IP là giao thức hướng nối (connection oriented)
- [x] IP là giao thức không hướng nối (connectionless oriented)

Câu 91. Khi Bob gửi email cho Alice, máy tính của Alice không kết nối mạng. Khi đó, email của Bob sẽ nằm ở đâu?
- [ ] Trong mail box của Bob trên mail server của Bob
- [ ] Trong hàng thư chờ gửi trên mail server của Alice
- [ ] Trong hàng thư chờ gửi trên mail server của Bob
- [x] Trong mail box của Alice trên mail server của Alice

Câu 92. Trong mạng cục bộ Ethernet, điều nào sau đây là đúng?
- [ ] Bên gửi vẫn tiếp tục gửi khung tin sau khi nghe được đụng độ
- [ ] Bên gửi dừng nghe đường truyền khi bắt đầu gửi khung tin
- [ ] Tín hiệu đụng độ được dùng để bổ trợ cho các khung tin với kích cỡ nhỏ
- [x] Thời gian chờ thay đổi theo thuật toán exponential backoff làm giảm xác suất đụng độ khi truyền lại

Câu 93. Được biết ngưỡng (threshold) hiện tại của quá trình kiểm soát tắc nghẽn là 16, hãy xác định giá trị của cửa sổ chống tắc nghẽn (congwin) khi bên gửi đã gửi tổng số 35 segment và nhận đầy đủ số ACK trả về mà không có bất kỳ lỗi nào 
- [ ] 19
- [ ] 18
- [ ] 16
- [x] 17

Câu 94. Địa chỉ IP của máy tính A là 110.2.112.12/20, địa chỉ IP của máy tính X là 110.2.109.4/20 và địa chỉ IP của máy tính Y là 110.2.105.20/20. Những máy tính nào có cùng địa chỉ mạng (subnet)?
- [x] Máy tính X và máy tính Y
- [ ] Máy tính X và máy tính A
- [ ] Cả 3 máy tính
- [ ] Máy tính A và máy tính Y

Câu 95. Một con số 32 bit, được sử dụng cùng địa chỉ IP của thiết bị để xác định địa
chỉ mạng (subnet) của thiết bị là
- [x] subnet mask
- [ ] ARP address
- [ ] DNS mask
- [ ] MAC address

Câu 96. Máy tính A gửi 1 gói tin IP cho máy tính B không nằm cùng một subnet. Hỏi
khung tin (frame) của layer 2 chứa gói tin IP khi gửi đi sẽ có địa chỉ MAC đích là địa
chỉ nào?
- [ ] Địa chỉ MAC của máy tính B
- [ ] Địa chỉ MAC của máy tính A
- [x] Địa chỉ MAC của router
- [ ] Địa chỉ MAC FF-FF-FF-FF

Câu 97. Giao thức UDP thường được dùng với ứng dụng nào sau đây?
- [ ] Ứng dụng thư điện tử
- [ ] Ứng dụng Web
- [ ] Ứng dụng truyền file
- [x] Ứng dụng nói chuyện trực tuyến (voice chat)

Câu 98. Máy tính A gửi cho máy tính B gói tin TCP thứ nhất có số thứ tự (sequence number) là 2000 và độ dài gói tin là 1000 byte, và gửi gói tin TCP thứ hai có số thứ tự là 3000 và độ dài gói tin là 200 byt- [ ] Tuy nhiên, máy tính B chỉ nhận được gói tin TCP thứ hai. Hỏi sau khi nhận gói tin TCP thứ hai, máy tính B gửi gói tin biên nhận ACK cho máy tính A với ACK bằng bao nhiêu?
- [ ] 3000
- [ ] 3200
- [x] 2000
- [ ] 1000

Câu 99. Một mạng LAN hình trạng bus có chiều dài 2km. Tốc độ lan truyền tín hiệu trên dây là 2 × 10 ^ 8 m/s. Mạng sử dụng CSMA/CD để truy nhập đường truyền và có tốc độ truyền dữ liệu là 10 ^ 7 bps . Trong CSMA/CD, người ta sử dụng cơ chế nghe đường truyền để phát hiện đụng độ (collision detection) trong khi vẫn đang truyền tin. Để máy phát hiện đụng độ trong khi truyền, thì tín hiệu sau khi đụng độ lại tiếp tục được truyền đi tiếp rồi quay lại máy đang truyền trong khoảng thời gian máy đang truyền tin. Trường hợp xấu nhất để máy truyền tín hiệu và tín hiệu lại quay trở về máy là hai lần khoảng thời gian lan truyền tín hiệu trong mạn- [ ] Khoảng thời gian này tương đương với việc máy truyền từ bit đầu tiên đến bit cuối cùng của khung tin. Như vậy, để đảm bảo mọi đụng độ đều có thể được phát hiện trong khi máy đang truyền tin thì kích cỡ nhỏ nhất của khung tin được sử dụng trong mạng LAN này nên là ?
- [ ] 50 bytes
- [ ] 100 bytes
- [ ] 200 bytes
- [x] 25 bytes

Câu 100. Điều nào sau đây đúng với giao thức định tuyến theo thuật toán distance vector ?
- [ ] Các bộ định tuyến trao đổi bảng định tuyến với nhau
- [x] Các bộ định tuyến trao đổi distance vector với các nút lân cận (neighbour node)
- [ ] Các bộ định tuyến không trao đổi thông tin với nhau
- [ ] Các bộ định tuyến sử dụng bảng định tuyến tĩnh

Câu 101. Trong giao thức CSMA/CD, nếu 2 máy tính cùng đồng thời truyền 2 khung tin vào môi trường truyền thì 2 máy tính này sẽ
- [ ] Tăng mức năng lượng của tín hiệu truyền để giảm nguy cơ bị lỗi do xung đột xảy ra
- [x] Phát hiện được xung đột và ngừng truyền dữ liệu ngay lập tức
- [ ] Gửi cảnh báo xung đột cho nhau và tiếp tục truyền
- [ ] Chỉ phát hiện được xung đột sau khi nhận được gói tin biên nhận ACK

Câu 102. Dịch vụ nào chuyển đổi tên miền và hostname sang địa chỉ IP
- [ ] Routing Information Protocol (RIP)
- [ ] Internet Relay Chat (IRC)
- [x] Domain Name System (DNS)
- [ ] Network Time Protocol (NTP)

Câu 103. Khi một gói tin rời khỏi mạng, Router NAT thay thế địa chỉ nguồn của gói tin đó bằng
- [ ] Địa chỉ port đích
- [ ] Không đáp án nào đúng
- [ ] Địa chỉ IP đích
- [x] Địa chỉ IP của NAT router

Câu 104. Bảng định tuyến của router A có các dòng được liệt kê như bên dưới, hãy cho biết nếu một gói tin có địa chỉ đích là 203.113.119.1 thì dòng nào sẽ được chọn để định tuyến cho gói tin đó
- [ ] Destination 203.113.0.0/16 → Gateway 193.168.10.1
- [x] Destination 203.113.64.0/18 → Gateway 113.57.10.1
- [ ] Destination 203.113.192.0/18 → Gateway 200.176.10.1
- [ ] Destination 203.113.128.0/17 → Gateway 14.8.10.1

Câu 105. Thiết bị kết nối mạng nào cho phép nhiều nút đồng thời cùng gửi và nhận trên các segment mạng khác nhau
- [ ] Repeater
- [x] Switch
- [ ] Hub
- [ ] Amplifier

Câu 105 - 106: Một gói tin có kích thước 2000 byte được truyền giữa hai máy tính trong mạng LAN. Biết khoảng cách vật lý giữa 2 máy tính là 400m, băng thông trong mạng LAN là 100 Mbps. Biết vận tốc lan truyền tín hiệu trong mạng LAN là 2x108 m/s.

Câu 105. Thời gian truyền dữ liệu (transmission time) vào mạng LAN là bao nhiêu?
- [ ] 0.00008 s
- [ ] 0.00001 s
- [ ] 0.00002 s
- [x] 0.00016 s

Câu 106. Thời gian lan truyền (propagation time) của gói tin giữa hai máy tính là bao nhiêu?
- [ ] 0.00004 s
- [ ] 0.000016 s
- [ ] 0.00001 s
- [x] 0.000002 s

Câu 107. Giả sử tốc độ lan truyền tín hiệu, tốc độ truyền dữ liệu từ A đến B lần lượt là 1km/s, 2Mbps. Khoảng cách giữa A và B là 2m, kích cỡ gói tin 50KB, Tiêu đề của gói tin chiếm 20% tổng kích cỡ gói tin. Thông lượng từ A đến B là xấp xỉ là bao nhiêu? Hãy chọn kết quả gần nhất sau đây 
- [ ] 1.7 Mbps
- [x] 1.6 Mbps
- [ ] 1.5 Mbps
- [ ] 1.4 Mbps

Câu 108. Router là thiết bị ở tầng
- [ ] Ứng dụng
- [ ] Liên kết dữ liệu
- [ ] Giao vận
- [x] Mạng

Câu 109. Tiến trình ứng dụng (application process) được đánh địa chỉ bởi
- [ ] Physical address
- [x] Port number
- [ ] Địa chỉ IP
- [ ] Process number

Câu 110. Phát biểu nào dưới đây về địa chỉ MAC là không đúng
- [ ] Địa chỉ MAC có chiều dài
- [x] Địa chỉ MAC được cấp phát thông qua giao thức ARP
- [ ] Địa chỉ MAC được sử dụng để gửi frame ở trong mạng nội bộ
- [ ] Địa chỉ MAC được biểu diễn sử dụng hệ "hexa"

Câu 111. Giao thức nào dưới đây là giao thức định tuyến kiểu trạng thái liên kết (link-state routing)?
- [ ] BGP
- [ ] RIP
- [ ] ICMP
- [x] OSPF

Câu 112. Giao thức để truyền trang web qua Internet là
- [ ] SSH
- [ ] DNS
- [ ] SMTP
- [x] HTTP

Câu 113. Khi sử dụng giao thức TCP, điều gì xảy ra nếu giá trị timeout được thiết lập quá nhỏ?
- [ ] Bên gửi sẽ nhận được gói tin ACK sớm hơn
- [x] Bên nhận sẽ nhận được nhiều gói tin TCP trùng lặp
- [x] Bên gửi sẽ phản ứng chậm với việc mất mát gói tin
- [ ] Buffer của bên nhận sẽ mau đây hơn

Câu 114. Các diễn đạt dưới đây về phương pháp xác định lỗi bít "single bit parity" ở tầng liên kết là "Đúng" hay "Sai"
- [x] Bit 1 được thêm vào cuối cùng sao cho tổng số bit 1 thu được là số lẻ
- [ ] Bit 0 được thêm vào đầu sao cho tổng số bit 0 tạo thành là số lẻ
- [x] Bit 1 được thêm vào cuối cùng sao cho tổng số bit 1 thu được là số chẵn
- [ ] Bit 0 được thêm vào đầu sao cho tổng số bit 0 tạo thành là số chẵn

Câu 115. Các phát biểu sau về CSMA, phát biểu nào sai
- [ ] Node sẽ không truyền frame nếu kênh truyền đang bận
- [x] Node dừng truyền frame ngay khi xung đột truy nhập kênh (collision) xảy ra
- [ ] Node muốn gửi dữ liệu sẽ cảm nhận sóng mang trên kênh trước khi truyền
- [ ] Xung đột có thể xảy ra do trễ lan truyền tín hiệu trên kênh

Câu 116. Giao thức dùng để tìm địa chỉ MAC nếu biết IP
- [x] ARP
- [ ] SSH
- [ ] DHCP
- [ ] Telnet

Câu 117. Frame là dữ liệu được trao đổi ở tầng
- [ ] Transport
- [x] Datalink
- [ ] Network
- [ ] Physical

Câu 118. Cho dữ liệu D= 100000, đa thức sinh G= 101. Mã CRC sẽ là :
- [ ] 11
- [x] 10
- [ ] 00
- [ ] 01

Câu 119. Hãy tìm câu trả lời đúng nhất liên quan đến thư điện tử
- [ ] SMTP là giao thức nhận thư điện tử
- [x] Bản ghi DNS kiểu MX dùng để chỉ tên miền và địa chỉ máy chủ thư điện tử
- [ ] POP3 và IMAP là các giao thức truyền thư điện tử
- [ ] Người dùng POP3 có thể xem lại lịch sử các thao tác đã thực hiện

Câu 120. Tốc độ của Gigabit Ethernet là bao nhiêu
- [x] 1000 Mb/s
- [ ] 10 Mb/s
- [ ] 1 Mb/s
- [ ] 100 Mb/s

Câu 121. Giao thức tự động gán địa chỉ IP cho máy tính
- [ ] FTP
- [x] DHCP
- [ ] WINS
- [ ] NAT

Câu 122. Chọn một phát biểu chính xác nhất
- [ ] OSPF là Inter-domain routing
- [x] Routing trên mạng Internet là kết hợp của các giao thức Inter-domain and Intra-domain
- [ ] RIP là giao thức routing phân cấp (hierarchical routing protocol)
- [ ] Giao thức định tuyến BGP sử dụng thuật toán routing Dijsktra

Câu 123. Máy tính A gửi 1 gói tin IP cho máy tính B không nằm cùng một subnet. Hỏi khung tin (frame) của layer 2 chứa gói tin IP khi gửi đi sẽ có địa chỉ MAC đích là địa chỉ nào?
- [x] Địa chỉ MAC của router
- [ ] Địa chỉ MAC FFFFFFFFFFF
- [ ] Địa chỉ MAC của máy tính B
- [ ] Địa chỉ MAC của máy tính A

Câu 124. Tầng phiên (Session) nhận dịch vụ từ tầng ... và sử dụng dịch vụ của tầng ......
- [x] presentation, transport
- [ ] application, presentation
- [ ] presentation, data link
- [ ] transport, network

Câu 125. Máy tính A gửi cho máy tính B một gói tin TCP thứ nhất có kích thước 200 byte và số thứ tự 120 và gói tin TCP thứ hai có kích thước 200 byt- [ ] Gói tin TCP thứ 2 đến trước và được lưu vào buffer, gói tin TCP thứ nhất đến sau. Hỏi sau khi nhận gói tin thứ nhất, máy tính B sẽ trả về gói tin ACK có sổ ACK (acknowledge number) là bao nhiêu?
- [ ] 420
- [ ] 122
- [ ] 320
- [x] 520

Câu 126. Các phát biểu dưới đây đúng hay sai ?
- [x] TCP sẽ tăng cửa sổ tắc nghẽn cũng lên 1 sau mỗi RTT khi ở giai đoạn congestion avoidance
- [ ] Ở giai đoạn slowstart, cửa sổ tắc nghẽn (congestion window - cwnd) tăng lên gấp đôi mỗi khi nhận được 1 ACK
- [x] Cả TCP và UDP đều có trường checksum trong phần tiêu đề
- [x] TCP header có thể có nhiều hơn 20 bytes
- [x] TCP header tối thiểu có 20 bytes
- [ ] TCP sẽ giảm cửa sổ cwnd đi một nửa khi phát hiện một gói bị mất do timeout 

Câu 127. Hãy xem xét một tình huống trong đó máy A đang truyền dữ liệu cho máy B.
- Segment đầu tiên A gửi cho B có Sequence Number bằng 10
- A gửi cho B tổng cộng 3 segments có kích thước tương ứng là: Segment-1: 100
bytes, segment2: 75 bytes, và segment-3: 90 bytes
- Việc gửi và nhận 3 gói là diễn ra theo thứ tự và không có lỗi
Hỏi: Sequence Number của segment-1, segment-2, segment-3 tương ứng là bao
nhiêu?
Chú ý: điền đáp án là 3 số nguyên cách nhau bằng dấu phẩy (,) và không có dấu
cách. Ví dụ: 10,15,2  
Ans: _10,110,185_

Câu 128. Một ứng dụng voice chat thời gian thực nên sử dụng giao thức nào dưới
đây?
- [x] UDP
- [ ] HTTP
- [ ] FTP
- [ ] TCP

Câu 129. 1 gói tin IP có độ dài 2000 byte, độ dài tiêu đề là 20 byt- [ ] Gói tin này được
truyền qua một liên kết vật lý có đơn vị dữ liệu lớn nhất (MTU) ở tầng IP là 500 byte
và bị phân mảnh. Hỏi giá trị của trường offset của mảnh thứ 2 là bao nhiêu?
- [ ] 125
- [x] 60
- [ ] 100
- [ ] 40

Câu 130. Trong một gói tin TCP (TCP segment), giá trị ACK number và Sequence Number là các số đếm, phản ánh:
- [ ] Không phải D, B, C
- [ ] Số thứ tự gói tin (tính theo segment) đang chờ nhận, và số thứ tự gói tin (segment) đang được truyền
- [ ] Giá trị cửa sổ nhận và giá trị cửa sổ truyền.
- [x] Số thứ tự (tính theo byte) đang chờ nhận, và số thứ tự tính theo byte, của byte đầu tiên của gói tin đang được truyền

Câu 131. Switch là thiết bị ở tầng
- [ ] Giao vận
- [ ] Ứng dụng
- [ ] Mạng
- [x] Liên kết dữ liệu

Câu 132. Hãy tìm câu trả lời không chính xác liên quan đến DHCP
- [ ] DHCP có thể trả lại địa chỉ của Default gateway (địa chỉ router đầu tiên)
- [ ] DHCP hoạt động ở tầng ứng dụng trong mô hình Internet
- [ ] Địa chỉ đích của gói tin DHCP Reply là 255.255.255.255
- [x] DHCP có thể sử dụng để truyền tin quảng bá

Câu 133. Các phát biểu dưới đây đúng hay sai ?
- [ ] Ứng dụng mạng chỉ có thể được kiến trúc theo kiểu client/server
- [x] Đặc điểm cơ bản của mô hình client/server là dựa trên cơ chế hỏi/đáp (request/response)
- [x] Ứng dụng mạng có thể được kiến trúc theo kiểu Peer-to-peer
- [x] Ứng dụng mạng có thể được kiến trúc theo kiểu Client/Server

Câu 134. Đặc điểm của TCP
- [ ] Không hướng nối
- [ ] Không tin cậy
- [ ] Hỗ trợ truyền quảng bá
- [x] Hướng nối

Câu 134. Máy tính A gửi cho máy tính B 3 gói tin TCP có cùng độ dài là 200 byte nhưng máy tính B chỉ nhận được đóng gói tin TCP thứ nhất và gói tin TCP thứ 3. Biết gói tin thứ nhất có số thứ tự (sequence number) là 1000, Hỏi gói tin biên nhận ACK mà máy tính B gửi trả cho máy tính A sau khi nhận gói tin thứ 3 có số biên nhận ACK là bao nhiêu?
- [x] 1200
- [ ] 1600
- [ ] 1400
- [ ] 1000

Câu 135. Trường địa chỉ port trong gói tin TCP có độ dài
- [x] 16 bit
- [ ] 32 bit

Câu 136. Trong mạng cục bộ Ethernet, điều nào sau đây là đúng?
- [ ] Bên gửi vẫn tiếp tục gửi khung tin sau khi nghe được đụng độ
- [ ] Tín hiệu đụng độ được dùng để bổ trợ cho các khung tin với kích cỡ nhỏ
- [ ] Bên gửi dừng nghe đường truyền khi bắt đầu gửi khung tin
- [x] Thời gian chờ thay đổi theo thuật toán exponential backoff làm giảm xác suất đụng độ khi truyền lại

Câu 137. Trên một mạng chuyển mạch gói, có một route (path) trải dài qua 3 kết nối vật lý (3 links). Trên route đó một file kích thước 1KBytes được gửi từ nút nguồn đến nút đích. Giả thiết rằng: (1) băng thông của tất cả các kết nối vật lý là 1Mbps; (2) trễ lan truyền tín hiệu (propagation delay) và trễ hàng đợi (queuing delay) là rất nhỏ; (3) đơn vị truyền dữ liệu của mạng là các gói tin bằng nhau kích thước 1000 byte; (4) Bỏ qua overhead của tất cả các giao thức sử dụng. Hỏi: Thời gian cần thiết để  truyền toàn bộ file đến đích là bao nhiêu miliseconds?  
Ans: _24_

Câu 138. Liên quan đến giao thức HTTP, hãy đánh dấu đúng sai vào các câu sau:
- [x] Header của bản tin HTTP có thể mang dữ liệu dạng nhị phân
- [x] Có hai bản tin HTTP là HTTP request và HTTP reply
- [x] HTTP có thể có nhiều dòng headers
- [ ] HTTP methods (ví dụ POST, GET, ...) tồn tại trong HTTP reply
- [ ] Bản tin HTTP luôn cần có phần payload
- [ ] HTTP status code tồn tại trong bản tin HTTP request
- [x] HTTP methods (ví dụ POST, GET, ...) tồn tại trong HTTP request
- [x] Payload của bản tin HTTP có thể mang dữ liệu dạng nhị phân
- [x] Phần tiêu đề (header) của giao thức HTTP có định dạng text

Câu 139. Những trường nào có trong header của frame Ethernet?
- [ ] authentication code
- [x] source and destination hardware addresses
- [ ] error correction code
- [ ] source and destination network addresses

Câu 140. Ba hình trang mạng được dùng phổ biến để nối kết các máy tính là: đường thẳng (bus), hình sao (Star with Switch), mạng vòng (ring). Theo anh/chị, trong trường hợp nào sau đây khi một máy tính truyền tin thì các máy khác đều có thể nhận được?
- [ ] Star with Switch và Ring
- [ ] Star with Switch và Star
- [x] Ring và Bus
- [ ] Star with Switch

Câu 141. Trong kiến trúc giao thức TCP/IP, tầng giao vận sử dụng dịch vụ gì của tầng mạng?
- [ ] Đảm bảo các gói tin đến bên nhận mà không có lỗi hoặc mất mát gói tin
- [ ] Đảm bảo các gói tin được truyền đến đúng tiến trình của bên nhận
- [ ] Đảm bảo không có tắc nghẽn trong mạng
- [x] Định tuyến gói tin đến đúng địa chỉ IP của bên nhận

Câu 142. Bảng định tuyến của router A có các dòng được liệt kê như bên dưới, hãy cho biết nếu một gói tin có địa chỉ đích là 203.113.119.1 thì dòng nào sẽ được chọn để định tuyến cho gói tin đó
- [ ] Destination 203.113.0.0/16 → Gateway 193.168.10.1
- [ ] Destination 203.113.128.0/17 → Gateway 14.8.10.1
- [x] Destination 203.113.64.0/18 - Gateway 113.57.10.1
- [ ] Destination 203.113.192.0/18 Gateway 200.176.10.1 

Câu 143. Các phát biểu dưới đây đúng hay sai ?
- [ ] POP3 và SMTP có chức năng tương đương
- [x] POP3 và IMAP có chức năng tương đương
- [x] Một hệ thống email có thể hoạt động được dựa vào POP3 và SMTP
- [x] Một hệ thống email có thể hoạt động được dựa vào IMAP và SMTP
- [x] Một hệ thống email có thể hoạt động được dựa vào HTTP và SMTP
- [ ] Một hệ thống email có thể hoạt động được dựa vào POP3 và IMAP
- [x] Hệ thống email hoạt động được cơ bản dựa vào hai loại giao thức: giao thức gửi mail và giao thức nhận mail
- [ ] Một hệ thống email có thể hoạt động được dựa vào POP3 và HTTP

Câu 144. Mạng Internet so các mạng điện thoại truyền thống (cố định, di động) có ưu điểm là
- [x] Sử dụng băng thông hiệu quả hơn
- [ ] Chất lượng truyền tin tốt hơn
- [ ] Độ trễ thấp hơn
- [ ] Bảo mật tốt hơn

Câu 145. Máy tính A gửi cho máy tính B gói tin TCP thứ nhất có số thứ tự (sequence number) là 2000 và độ dài gói tin là 1000 byte, và gửi gói tin TCP thứ hai có số thứ tự là 3000 và độ dài gói tin là 200 byt- [ ] Tuy nhiên, máy tính B chỉ nhận được gói tin TCP thứ hai. Hỏi sau khi nhận gói tin TCP thứ hai, máy tính B gửi gói tin biên nhận ACK cho máy tính A với ACK bằng bao nhiêu?
- [ ] 3200
- [ ] 1000
- [ ] 3000
- [x] 2000

Câu 146. Lợi ích của việc mạng nội bộ dùng NAT là
- [ ] NAT giúp việc gán địa chỉ IP cho từng thiết bị nhanh hơn.
- [x] Chỉ cần sử dụng một địa chỉ IP cho tất cả các thiết bị trong mạng
- [x] Có thể thay đổi ISP một cách dễ dàng mà không cần thay đổi địa chỉ IP của các thiết bị trong mạng
- [ ] Các thiết bị trong mạng có thể gửi trực tiếp data cho nhau mà không cần địa chỉ IP

Câu 147. Ưu điểm của thiết bị hub so với thiết bị switch (layer 2) là gì?
- [x] Đơn giản, dễ chế tạo
- [ ] Có khả năng định tuyến ở tầng IP
- [ ] Có khả năng kết nối các cổng LAN có tốc độ truyền khác nhau
- [ ] Phân chia mạng LAN thành các miền xung đột khác nhau

Câu 148. Địa chỉ IP loopback là
- [ ] 255.255.255.255
- [x] 127.0.0.1
- [ ] 192.168.1.1
- [ ] 10.10.10.10

Câu 149. Chọn ý đúng trong các diễn đạt dưới đây về cơ chế store-and-forward ở router
- [ ] Gói tin được forward theo từng byte, cứ byte nào vào thì forward by đó ra
- [ ] Chỉ cần header của gói tin đến router là có thể forward gói tin đi tiếp luôn
- [ ] Cứ bit nào vào là có thể forward bit đó ra luôn
- [x] Toàn bộ gói tin phải đến router trước khi nó có thể được forward đi tiếp

Câu 150. Bộ giao thức truyền dữ liệu qua Internet là?
- [ ] VoiceIP
- [ ] DNS
- [ ] HTTP
- [x] TCP/IP

Câu 151. Trong các tài liệu về mạng máy tính hiện nay, các tác giả hay sử dụng các ví dụ dựa trên mạng để trình bày Internet để có tính thực tế. Để có tính lý thuyết cao, họ cũng thường sử dụng mô hình ... (có 7 tầng)  
Ans: _OSI_

Câu 152. Tại sao giao thức HTTP lại sử dụng giao thức TCP mà không sử dụng giao thức UDP để truyền dữ liệu?
- [ ] Giao thức TCP có độ trễ thấp hơn
- [ ] Giao thức TCP có tốc độ truyền cao hơn
- [ ] Giao thức TCP có cơ chế truyền dữ liệu đơn giản, ít dư thừa hơn
- [x] Giao thức TCP đảm bảo truyền tin tin cậy.

Câu 152. Dữ liệu khi truyền từ máy tính A và máy tính B cần đi qua 3 đường truyền vật lý có băng thông lần lượt là 10Mbps, 20Mbps và 30 Mbps. Hỏi tốc độ truyền dữ liệu tối đa giữa A và B là bao nhiêu? 
- [x] 10Mbps
- [ ] 30Mbps
- [ ] Không đáp án nào trong 3 đáp án A, D và B là đúng
- [ ] 20Mbps

Câu 153.
1. Cho sơ đồ mạng sau:
R1----->subnet A---->R2-----subnet B------>Máy tính H.
Gói tin P có kích cỡ 2000 bytes (là gói tin TCP gồm phần tiêu đề và dữ liệu) được gửi từ bộ định tuyến R1 đến máy tính H thông qua subnet A và subnet B với trung gian là bộ định tuyến R2. MTU của subnet A và subnet B lần lượt là 1500 bytes và 532 bytes. Kích cỡ tiêu đề IP là 20bytes. Khi P đi qua subnet A, P được chia thành 2 mảnh với bit M (fragflag) và offset của các mảnh lần lượt như sau:
- [x] M=1, offset=0; M=0, offset=185
- [ ] M=1, offset=0;M=0, offset=1481
- [ ] M=0, offset=0;M=1, offset=1480
- [ ] M=1, offset=0; M=0, offset=1480

Câu 154. Các phát biểu dưới đây là đúng hay sai
- [ ] Một trong hai chức năng chính của mạng lõi (network core) là điều khiển đa truy cập (Multiple Access).
- [ ] Một trong hai chức năng chính của mạng lõi (network core) là phát hiện lỗi (Error detection)
- [x] Một trong hai chức năng chính của mạng lõi (network core) là định tuyến (Routing)
- [x] Một trong hai chức năng chính của mạng lõi (network core) là chuyển tiếp gói tin (Forwarding)
Câu 155. HTTP server nghe ở port nào
- [ ] 81
- [x] 80
- [ ] 25
- [ ] 82
Câu 156. Hiện tượng mất dữ liệu (loss) xảy ra trên mạng truyền dữ liệu (data networks) chủ yếu do nguyên nhân nào?
- [ ] Mất gói tin do vượt quá giá trị TTL (Time To Live)
- [ ] Cả D, C, A
- [x] Mất gói tin do tràn bộ đệm
- [ ] Mất gói tin do lỗi bit trên đường truyền

Câu 157. Trong một mạng LAN có cài đặt một switch nối với một router. Router được tích hợp chức năng DHCP và DNS. Một máy tính (máy C) được cấu hình sử dụng DHCP được bật lên và cắm vào switch của mạn- [ ] Ngay sau khi máy C được cấp phát thành công một địa chỉ IP, C thực hiện một câu truy vấn tên miền www.vnexpress.net đến máy chủ DNS nội bộ của mạng LAN. Giả sử rằng tên miền www.vnexpress.net đã được cache tại máy chủ DNS nội bộ. Hỏi: Câu nào chính xác nhất trong các phát biểu dưới đây?
- [ ] Sau khi máy C cắm vào switch, ARP được kích hoạt ở lớp datalink, sau đó DHCP được kích hoạt, sau đó DNS được kích hoạt ở tầng ứng dụng
- [ ] Sau khi máy C cắm vào switch, DHCP được kích hoạt, sau đó DNS được kích hoạt ở tầng ứng dụng khiến cho ARP được kích hoạt ở tầng datalink.
- [x] Sau khi máy C cắm vào switch, DHCP được kích hoạt chạy bên trên UDP, sau đó ARP được kích hoạt ở lớp datalink, sau đó DNS chạy ở tầng ứng dụng để có được tên miền www.vnexpress.net
- [ ] Sau khi máy C cắm vào switch, DNS được kích hoạt ở tầng ứng dụng, sau đó DHCP được kích hoạt sử dụng UDP ở tầng giao vận, sau đó ARP được kích hoạt ở tầng datalink

Câu 158. Giao thức nào gửi yêu cầu quảng bá (broadcast) và nhận phản hồi đơn điểm (unicast):
- [x] ARP
- [ ] CSMA/CD
- [ ] TCP
- [ ] ICMP

Câu 159. Trong các phát biểu sau về kiến trúc Client-Server, câu nào kém chính xác nhất
- [ ] Server thường phải có địa chỉ và port cố định
- [ ] Client có thể gửi bản tin Request đến server
- [x] Client có thể không là bên bắt đầu quá trình liên lạc
- [ ] Client-Server hoạt động dựa chủ yếu dựa trên cơ chế request reply

Câu 160. Máy chủ DNS A quản lý domain name là vn. Máy chủ DNS B quản lý domain name là edu.vn. Máy chủ DNS C quản lý domain name là vnu.edu.vn. Máy chủ DNS D quản lý domain name là uet.vnu.edu.vn. Máy chủ nào là máy chủ DNS có thẩm quyền (authoritative DNS server) đối với tên miền fit.uet.vnu.edu.vn? 
- [x] Máy chủ DNS D
- [ ] Máy chủ DNS B
- [ ] Máy chủ DNS A
- [ ] Máy chủ DNS C

Câu 161. Máy tính A và B truyền dữ liệu qua giao thức TCP. Khi máy tính A nhận định có tắc nghẽn xảy ra trong mạng, máy tính A sẽ
- [x] Giảm tốc độ truyền dữ liệu bằng cách giảm kích thước cửa sổ gửi
- [ ] Dừng gửi dữ liệu cho đến khi router báo hết tắc nghẽn
- [ ] Dừng gửi dữ liệu cho đến khi máy tính B gửi gói tin ACK báo hết tắc nghẽn
- [ ] Tăng tốc độ truyền dữ liệu để bù lại lượng dữ liệu mất mát do tắc nghẽn

Câu 162. Core network của mạng Internet sử dụng cơ chế
- [ ] Circuit switching
- [x] Packet switching
- [ ] Label switching
- [ ] Datagram switching

Câu 163. Giao thức HTTP sử dụng công ngầm định nào?
- [ ] 40
- [x] 80
- [ ] 10
- [ ] 20

Câu 164. Các phát biểu dưới đây là đúng hay sai
- [ ] DNS root name server là nơi lưu trữ toàn bộ thông tin về cặp (hostname, địa chỉ IP)
- [ ] DNS là giao thức ở tầng transport
- [ ] DNS cung cấp dịch vụ chuyển đổi địa chỉ IP sang MAC
- [x] DNS cung cấp dịch vụ chuyển đổi hostname sang địa chỉ IP

Câu 165. ACK được sử dụng để làm gì trong giao thức truyền dữ liệu đáng tin cậy (reliable data transfer protocol) ở tầng transport
- [ ] Là cơ chế giúp sửa lỗi bit gói tin khi nhận
- [ ] Là cơ chế giúp khôi phục gói tin bị mất
- [ ] Cả 3 đáp án đều sai
- [x] Là cơ chế thông báo tình trạng nhận gói tin

Câu 166. Địa chỉ IPv4 có bao nhiêu bit
- [ ] 8
- [x] 32
- [ ] 128
- [ ] 2

Câu 167. Các tầng tương tác với
- [ ] Tầng dưới nó
- [ ] Mọi tầng khác
- [x] Tầng trên và tầng dưới
- [ ] Tầng dưới nó

Câu 168. Trong các phương thức dưới đây, phương thức nào là phương thức của HTTP?
- [ ] VIEW
- [ ] RUN
- [x] POST
- [x] HEAD
- [x] GET
- [ ] REMOVE
- [x] PUT

Câu 169. Phát biểu nào dưới đây không đúng về thiết bị switch
- [ ] Switch sử dụng forwarding table để forward frame
- [x] Switch hoạt động ở tầng vật lý
- [ ] Switch hoạt động theo cơ chế store và forward
- [ ] Switch xây dựng forwarding table theo cơ chế tự học

Câu 170. OSPF là giao thức nào dưới đây?
- [ ] Giao thức định tuyến trong mạng chuyển mạch ảo (Virtual circuit routing)
- [ ] Giao thức định tuyến trong mạng LAN
- [x] Giao thức định tuyến trong miền tự trị (intra AS)
- [ ] Giao thức định tuyến giữa các miền tự trị (inter AS)

Câu 171. Hãy tìm câu trả lời đúng nhất liên quan đến DNS:
- [ ] Dịch vụ DNS trả lại địa chỉ IP dùng riêng (private IP)
- [ ] DNS chỉ sử dụng giao thức UDP ở tầng giao vận
- [ ] DNS phân giải địa chỉ vật lý thành địa chỉ IP
- [x] Một máy chủ DNS có thể quản lý nhiều miền khác nhau

Câu 172. Một router nhận một gói tin IP có độ dài phần dữ liệu là 1000 byte và định tuyến gói tin này qua một liên kết mạng có MTU là 500 byt- [ ] Gói tin IP không có trường option. Trường length của gói bé nhất có giá trị bao nhiêu ? 
- [ ] 80
- [x] 60
- [ ] 40
- [ ] 20

Câu 173. Cơ cấu chuyển mạch (switching fabric) nào sau đây có tốc độ xử lý gói tin nhanh nhất ? Biết tốc độ xử lý của các đường bus là như nhau.
- [x] Kiểu cross-bar
- [ ] Kiểu memory
- [ ] Kiểu store-and-forward
- [ ] Kiểu bus

Câu 174. Máy tính A gửi 1 gói tin IP cho máy tính B không nằm cùng một subnet. Hỏi khung tin (frame) của layer 2 chứa gói tin IP khi gửi đi sẽ có địa chỉ MAC đích là địa chỉ nào?
- [ ] Địa chỉ MAC của máy tính A
- [ ] Địa chỉ MAC của máy tính B
- [ ] Địa chỉ MAC FF-FF-FF-FF
- [x] Địa chỉ MAC của router

Câu 175. Một máy tính có địa chỉ IP là 192.168.1.2 và Subnet mask là 255.255.255.0. Mạng này có thể có tối đa bao nhiêu máy tính có địa chỉ IP riêng (chú ý phần host không thể gồm toàn 0 hoặc toàn 1 
- [x] 254
- [ ] 255
- [ ] 8
- [ ] 256

Câu 176. Tầng giao vận (Transport layer) cung cấp một kết nối giữa các
- [x] Process
- [ ] Host
- [ ] End system
- [ ] Router

Câu 177. Phát biểu nào sau đây không chính xác về giao thức ARP
- [ ] ARP hoạt động dựa trên ARP table
- [x] ARP không sử dụng phương thức truyền broadcast trong LAN
- [ ] ARP là giao thức hoạt động theo kiểu Request/reply
- [ ] ARP phân giải địa chỉ IP ra địa chỉ MAC

Câu 178. Khi Bob gửi mail đến Alice, giao thức SMTP được sử dụng để chuyển mail của Bob đến
- [x] Hòm thư (mail box) trên máy chủ của Alice
- [ ] Hàng đợi thông báo (message queue) trên máy chủ của Bob
- [ ] Cả hai ý A và B
- [ ] Trình đọc mail (User agent) của Alice

Câu 179. Trong một mạng LAN có cài đặt một switch nối với một router. Router được tích hợp chức năng DHCP và DNS. Một máy tính (máy C) được cấu hình sử dụng DHCP được bật lên và cắm vào switch của mạn- [ ] Ngay sau khi máy C được cấp phát thành công một địa chỉ IP, C thực hiện một câu truy vấn tên miền www.vnexpress.net đến máy chủ DNS nội bộ của mạng LAN. Giả sử rằng tên miền www.vnexpress.net đã được cache tại máy chủ DNS nội bộ. 
Hỏi: Câu nào chính xác nhất trong các phát biểu dưới đây?
- [ ] Sau khi máy C cắm vào switch, DHCP được kích hoạt chạy bên trên UDP, sau đó ARP được kích hoạt ở lớp datalink, sau đó DNS chạy ở tầng ứng dụng để có được tên miền www.vnexpress.net
- [ ] Sau khi máy C cắm vào switch, ARP được kích hoạt ở lớp datalink, sau đó DHCP được kích hoạt, sau đó DNS được kích hoạt ở tầng ứng dụng
- [ ] Sau khi máy C cắm vào switch, DNS được kích hoạt ở tầng ứng dụng, sau đó DHCP được kích hoạt sử dụng UDP ở tầng giao vận, sau đó ARP được kích hoạt ở tầng datalink
- [ ] Sau khi máy C cắm vào switch, DHCP được kích hoạt, sau đó DNS được kích hoạt ở tầng ứng dụng khiến cho ARP được kích hoạt ở tầng datalink. 

Câu 180. Bảng thông tin chuyển tiếp của một bộ định tuyến như sau. Bộ định tuyến nhận được ba gói tin IPv4 từ máy 10.10.10.1 gửi lần lượt đến các máy 192.168.1.1, 172.16.2.9, 172.5.16.1. Khi đó các gói tin này sẽ được gửi tới các cổng ra tương ứng của bộ định tuyến: 

|Destination |Output port|
|-|-|
|192.168.1.0/24 |A|
|192.168.1.0/30 |B|
|172.16.0.0/16 |C|
|172.16.2.0/24 |D|
|172.16.2.128/25 |E|
|0.0.0.0/0 |F|
- [x] B, D, F
- [ ] A, E, F
- [ ] B, D, E
- [ ] A, C, E

Câu 181. Máy tính A muốn gửi 1 gói tin IP cho máy tính B có địa chỉ IP cho trước nhưng không biết địa chỉ MAC của máy tính B. Máy tính A sẽ
- [ ] Gửi gói tin IP đi với địa chỉ MAC đích là FF:FF:FF:FF
- [ ] Gửi gói tin IP đi với địa chỉ MAC đích là 00:00:00:00
- [ ] Gửi truy vấn DNS để biết địa chỉ MAC của máy tính B
- [x] Sử dụng giao thức ARP để truy vấn địa chỉ MAC của máy tính B

Câu 182. Tại sao giao thức HTTP lại sử dụng giao thức TCP mà không sử dụng giao thức UDP để truyền dữ liệu?
- [x] Giao thức TCP đảm bảo truyền tin tin cậy
- [ ] Giao thức TCP có cơ chế truyền dữ liệu đơn giản, ít dư thừa hơn
- [ ] Giao thức TCP có độ trễ thấp hơn
- [ ] Giao thức TCP có tốc độ truyền cao hơn

Câu 183. Trên một mạng chuyển mạch gói, có một route (path) trải dài qua 3 kết nối vật lý (3 links). Trên router đó một file kích thước 1KBytes được gửi từ nút nguồn đến nút đích. Giả thiết rằng: 
(1) băng thông của tất cả các kết nối vật lý là 1Mbps; 
(2) trễ lan truyền tín hiệu (propagation delay) và trễ hàng đợi (queuing delay) là rất nhỏ; 
(3) đơn vị truyền dữ liệu của mạng là các gói tin bằng nhau kích thước 1000 byte;
(4) Bỏ qua overhead của tất cả các giao thức sử dụng.
Hỏi: Thời gian cần thiết để truyền toàn bộ file đến đích là bao nhiêu miliseconds?  
Ans: _24_

Câu 184. Đặc điểm của UDP là
- [ ] Quảng bá
- [x] Không hướng nối
- [ ] Hướng nối
- [ ] Tin cậy

Câu 185. Mail từ máy tính người gửi được gửi trực tiếp đến chương trình đọc thư
trên máy tính người đọc.
- [ ] Đúng
- [x] Sai

Câu 186. So với mô hình OSI, mô hình TCP/IP có hay không có các tầng nào dưới
đây
- [x] Tầng ứng dụng (application layer)
- [x] Tầng vật lý(Physical layer)
- [x] Tầng liên kết (link layer)
- [ ] Tầng phiên (session layer)
- [ ] Tầng trình diễn (presentation layer)
- [x] Tầng giao vận (transport layer)
- [x] Tầng mạng (network layer)

Câu 187. Tham số cửa sổ tắc nghẽn (cwnd) trong giao thức TCP là một đại lượng nguyên, đo bằng đơn vị
- [ ] Số lượng TCP segments (number of TCP segments)
- [ ] Số lượng Byte dữ liệu
- [x] Số lượng MSS (number of MSS - Maximum Segment Size)
- [ ] Không có đơn vị

Câu 188. Chọn một phát biểu chính xác nhất
- [ ] RIP là giao thức routing phân cấp (hierarchical routing protocol)
- [ ] OSPF là Inter-domain routing
- [ ] Giao thức định tuyến BGP sử dụng thuật toán routing Dijkstra
- [x] Routing trên mạng Internet là kết hợp của các giao thức Inter-domain and Intra-domain

Câu 189. Frame là dữ liệu được trao đổi ở tầng
- [ ] Network
- [x] Datalink
- [ ] Transport
- [ ] Physical

Câu 190. CSMA/CD thuộc kiểu giao thức truy cập môi trường nào
- [x] Random Access
- [ ] Taking turn
- [ ] Channel Partitioning

Câu 191. Độ trễ lan truyền (Propagation delay) phụ thuộc vào
- [x] Khoảng cách vật lý giữa bên gửi và bên nhận
- [ ] Kích thước gói tin
- [ ] Băng thông của đường truyền vật lý giữa bên gửi và bên nhận
- [ ] Kích thước hàng đợi tại router

Câu 192. Máy tính A gửi cho máy tính B dữ liệu là chuỗi bit 11010. Tìm mã kiểm tra lỗi CRC biết biết máy tính A sử dụng đa thức sinh (generator) là 101  
Ans: _01_

Câu 193. Dịch vụ nào chuyển đổi tên miền và hostname sang địa chỉ IP
- [ ] Internet Relay Chat (IRC)
- [ ] Network Time Protocol (NTP)
- [x] Domain Name System (DNS)
- [ ] Routing Information Protocol (RIP)

Câu 194. Khi Bob gửi mail đến Alice có địa chỉ alice@hogehoge.com, để biết được mail server của Alice thì mail server của Bob gửi truy vấn DNS như thế nào?
- [ ] Gửi truy vấn tên miền hogehoge.com với type=NS
- [x] Gửi truy vấn tên miền hogehoge.com với type=MX
- [ ] Gửi truy vấn tên miền hogehoge.com với type=CNAME
- [ ] Gửi truy vấn tên miền hogehoge.com với type=A

Câu 195. Câu nào diễn đạt đúng về giao thức IP?
- [x] IP là giao thức không hướng nối (connectionless oriented)
- [ ] IP là giao thức đảm bảo thời gian thực
- [ ] IP là giao thức tin cậy
- [ ] IP là giao thức hướng nối (connection oriented)

Câu 196. Các phát biểu dưới đây là đúng hay sai
- [ ] Nội dung lựa chọn
- [x] DNS cung cấp dịch vụ chuyển đổi hostname sang địa chỉ IP
- [ ] CÁC MỤC
- [ ] 2

Câu 197. Gói SYNACK được gửi khi muốn thiết lập kết nối TCP
- [ ] Đúng
- [x] Sai

Câu 198. HTTP server nghe ở port nào
- [ ] 81
- [ ] 25
- [ ] 82
- [x] 80

Câu 199. Hãy xem xét việc truyền dữ liệu trên một kênh truyền vật lý. Nguyên nhân
mất dữ liệu xảy ra trên kênh chủ yếu là do
- [x] Mất dữ liệu do tràn bộ đệm
- [ ] Lỗi bit tín hiệu
- [ ] Cả A, D và B
- [ ] Mất gói tin do vượt quá số lượt forward của package (TTL)

Câu 200. Trong giao thức CSMA/CD, nếu 2 máy tính cùng đồng thời truyền 2 khung tin vào môi trường truyền thì 2 máy tính này sẽ
- [x] Phát hiện được xung đột và ngừng truyền dữ liệu ngay lập tức
- [ ] Chỉ phát hiện được xung đột sau khi nhận được gói tin biên nhận ACK
- [ ] Tăng mức năng lượng của tín hiệu truyền để giảm nguy cơ bị lỗi do xung đột xảy ra
- [ ] Gửi cảnh báo xung đột cho nhau và tiếp tục truyền

Câu 201. Tại sao phải dùng số thứ tự trong giao thức truyền dữ liệu tin cậy ở tầng transport (reliable data transfer protocol)
- [ ] Để thống kê được số gói tin đã gửi đi
- [ ] Để thống kê được số gói tin đã nhận được
- [x] Để tránh dữ liệu bị trùng lặp ở phía nhận do gửi lại nhiều lần
- [ ] Để tránh việc một gói tin được gửi lại nhiều lần

Câu 202. Mạng máy tính là
- [ ] Tập hợp các máy tính trong một phòng
- [x] Nhiều máy tính có kết nối với nhau
- [ ] Một kiểu máy tính

Câu 203. Trong các phát biểu sau về kiến trúc Client-Server, câu nào kém chính xác nhất
- [ ] Server thường phải có địa chỉ và port cố định
- [ ] Client-Server hoạt động dựa chủ yếu dựa trên cơ chế request/reply
- [ ] Client có thể gửi bản tin Request đến server
- [x] Client có thể không là bên bắt đầu quá trình liên lạc

Câu 204. OSPF là giao thức nào dưới đây?
- [ ] Giao thức định tuyến giữa các miền tự trị (inter AS)
- [ ] Giao thức định tuyến trong mạng LAN
- [ ] Giao thức định tuyến trong mạng chuyển mạch ảo (Virtual circuit routing)
- [x] Giao thức định tuyến trong miền tự trị (intra AS)

Câu 205. Máy tính A gửi cho máy tính B một gói tin TCP thứ nhất có kích thước 200 byte và số thứ tự 120 và gói tin TCP thứ hai có kích thước 200 byte. Gói tin TCP thứ 2 đến trước và được lưu vào buffer, gói tin TCP thứ nhất đến sau. Hỏi sau khi nhận gói tin thứ nhất, máy tính B sẽ trả về gói tin ACK có số ACK (acknowledge number) là bao nhiêu?
- [ ] 320
- [ ] 122
- [x] 520
- [ ] 420

Câu 206. Giao thức TCP quy định gói tin sai số thứ tự phải bị xóa bỏ
- [ ] Sai
- [ ] Đúng
- [x] Tùy phiên bản giao thức TCP

Câu 207. Phương pháp đa truy cập nào dưới đây không thuộc nhóm giao thức "truy cập ngẫu nhiên (random access)
- [x] FDMA
- [ ] CSMA/CD
- [ ] ALOHA
- [ ] CSMA

Câu 208. Số lượng Root Name Server trong hệ thống DNS gần giá trị nào nhất
- [ ] 100
- [ ] 2
- [x] 13
- [ ] 1000

Câu 209. Hãy tìm câu trả lời đúng nhất liên quan đến HTTP
- [x] Nếu nhận được HTTP request có nội dung If-modified-since trong phần tiêu đề, máy chủ HTTP sẽ chỉ trả lại nội dung được yêu cầu với mã 200 nếu như nội dung đó được cập nhật lần cuối sau ngày được đưa ra
- [ ] Máy chủ thường phục vụ HTTP trên cổng 80,808 và 8080
- [ ] HTTP quy định hoạt động của các nút bấm trên một trình duyệt Web
- [ ] HTTP quy định cách hiển thị các hình ảnh trên một trình duyệt Web

Câu 210. Trong một gói tin TCP (TCP segment), giá trị ACK number và Sequence Number là các số đếm, phản ánh:
- [x] Số thứ tự (tính theo byte) đang chờ nhận, và số thứ tự tính theo byte, của byte đầu tiên của gói tin đang được truyền
- [ ] Không phải A, C, D
- [ ] Số thứ tự gói tin (tính theo segment) đang chờ nhận, và số thứ tự gói tin (segment) đang được truyền
- [ ] Giá trị cửa sổ nhận và giá trị cửa sổ truyền

Câu 211. Được biết ngưỡng (threshold) hiện tại của quá trình kiểm soát tắc nghẽn là 16, hãy xác định giá trị của cửa sổ chống tắc nghẽn (congwin) khi bên gửi đã gửi tổng số 35 segment và nhận đầy đủ số ACK trả về mà không có bất kỳ lỗi nào 
- [ ] 19
- [ ] 18
- [ ] 16
- [x] 17

Câu 212. Thiết bị kết nối mạng nào cho phép nhiều nút đồng thời cùng gửi và nhận
trên các segment mạng khác nhau
- [ ] Amplifier
- [ ] Hub
- [ ] Repeater
- [x] Switch

Câu 213. Các phát biểu dưới đây là đúng hay sai
- [ ] FTP sử dụng giao thức UDP
- [ ] DNS sử dụng giao thức TCP
- [ ] SMTP sử dụng giao thức UDP
- [x] HTTP sử dụng giao thức TCP

Câu 214. Chọn ý đúng trong các diễn đạt dưới đây về cơ chế store-and-forward ở router
- [ ] Gói tin được forward theo từng byte, cứ byte nào vào thì forward by đó ra
- [ ] Cứ bit nào vào là có thể forward bit đó ra luôn
- [x] Toàn bộ gói tin phải đến router trước khi nó có thể được forward đi tiếp
- [ ] Chỉ cần header của gói tin đến router là có thể forward gói tin đi tiếp luôn

Câu 215. Trong mạng cục bộ Ethernet, điều nào sau đây là đúng?
- [ ] Bên gửi vẫn tiếp tục gửi khung tin sau khi nghe được đụng độ
- [x] Thời gian chờ thay đổi theo thuật toán exponential backoff làm giảm xác suất đụng độ khi truyền lại
- [ ] Tín hiệu đụng độ được dùng để bổ trợ cho các khung tin với kích cỡ nhỏ
- [ ] Bên gửi dừng nghe đường truyền khi bắt đầu gửi khung tin

Câu 216. Với lập trình socket, người lập trình không quan tâm việc Hệ điều hành sử dụng giao thức giao vận TCP hay UDP như thế nào. Đúng hay sai?
- [x] Sai
- [ ] Đúng

Câu 217. Giao thức UDP thường được dùng với ứng dụng nào sau đây?
- [ ] Ứng dụng Web
- [ ] Ứng dụng thư điện tử
- [x] Ứng dụng nói chuyện trực tuyến (voice chat)
- [ ] Ứng dụng truyền file

Câu 218. Phát biểu nào dưới đây không đúng về thiết bị switch
- [ ] Switch hoạt động theo cơ chế store và forward
- [ ] Switch sử dụng forwarding table để forward frame
- [x] Switch hoạt động ở tầng vật lý
- [ ] Switch xây dựng forwarding table theo cơ chế tự học

Câu 219. Máy tính A và B truyền dữ liệu qua giao thức TCP. Khi máy tính A nhận định có tắc nghẽn xảy ra trong mạng, máy tính A sẽ
- [x] Giảm tốc độ truyền dữ liệu bằng cách giảm kích thước cửa sổ gửi
- [ ] Dừng gửi dữ liệu cho đến khi router báo hết tắc nghẽn
- [ ] Dừng gửi dữ liệu cho đến khi máy tính B gửi gói tin ACK báo hết tắc nghẽn
- [ ] Tăng tốc độ truyền dữ liệu để bù lại lượng dữ liệu mất mát do tắc nghẽn

Câu 220. Ý nào dưới đây không đúng về giao thức OSPF
- [ ] OSPF sử dụng thuật toán định tuyến link-state
- [ ] OSPF mã hóa các OSPF message
- [x] OSPF không cho phép chọn nhiều path có cost giống nhau
- [ ] OSPF ho tro dinh tuyen phan cap

Câu 221. Một gói tin IP sau khi gửi có thể không đến được bên nhận. Tại sao?
- [x] Tất cả các đáp án đều đúng
- [ ] Gói tin bị loại bỏ do tràn bộ đệm ở router
- [ ] Gói tin bị loại bỏ do đi hết số chặng định tuyến theo quy định
- [ ] Gói tin bị loại bỏ do có lỗi bit

Câu 222. Dữ liệu khi truyền từ máy tính A và máy tính B cần đi qua 3 đường truyền vật lý có băng thông lần lượt là 10Mbps, 20Mbps và 30 Mbps. Hỏi tốc độ truyền dữ liệu tối đa giữa A và B là bao nhiêu?
- [ ] 30Mbps
- [x] 10Mbps
- [ ] Không đáp án nào trong 3 đáp án B, D và A là đúng
- [ ] 20Mbps

Câu 223. Tầng datalink sử dụng .... để chuyển gói tin đến đích
- [ ] Địa chỉ IP
- [ ] Cổng
- [ ] Tên máy tính
- [x] Địa chỉ MAC

Câu 224. Core network của mạng Internet sử dụng cơ chế
- [ ] Circuit switching
- [ ] Datagram switching
- [x] Packet switching
- [ ] Label switching

Câu 225. Tốc độ của Gigabit Ethernet là bao nhiêu
- [ ] 10 Mb/s
- [ ] 1 Mb/s
- [ ] 100 Mb/s
- [x] 1000 Mb/s

Câu 226. Mạng cục bộ LAN là viết tắt của
- [x] Local Area Network
- [ ] Local Arial Net
- [ ] Low Area Network

Câu 227. Mạng Internet là một mạng có cấu trúc như thế nào?
- [ ] Client - Server
- [x] Phân cấp
- [ ] Peer-to-peer
- [ ] Phẳng

Câu 228. Giao thức dùng để gửi email giữa cái mail server là
- [ ] IMAP
- [x] SMTP
- [ ] FTP
- [ ] POP3

Câu 229. Địa chỉ IP loopback là
- [x] 127.0.0.1
- [ ] 192.168.1.1
- [ ] 10.10.10.10
- [ ] 255.255.255.255

Câu 230. Địa chỉ MAC có chiều dài
- [x] 48 bit
- [ ] 32 bit
- [ ] 16 bit

Câu 231. Những phát biểu dưới đây đúng hay sai
- [x] Giao thức TCP có tính chất công bằng (fairness) là nhờ chiến lược điều khiển tắc nghẽn theo kiểu AIMD (Additive Increase Multiplicative Decrease)
- [ ] Gỉa sử một mạng có dung lượng là 64 Kbps, trên đó chỉ có 1 kết nối TCP. Khi kết nối TCP đó được mở và dữ liệu được truyền trên đó, thông lượng dữ liệu (throughput) của kết nối đó ngay lập tức bằng 64Kbps
- [ ] Giao thức TCP phát hiện ra gói bị mất nhờ vào trường checksum
- [ ] Các TCP segments là luôn luôn có phần payload
- [x] Kích thước phần tiêu đề (header) của TCP là lớn hơn kích thước tiêu đề của UDP
- [ ] Kích thước phần tiêu đề của UDP bằng 20 bytes
- [ ] Mỗi kết nối TCP chỉ cho phép truyền dữ liệu một chiều từ bên gửi đến bên nhận
- [x] Nếu mạng có dung lượng 2Mbps, trên đó có 2 kết nối TCP chạy song song, thì thông lượng trung bình của mỗi kết nối TCP sẽ chiếm xấp xỉ 1Mbps
- [ ] Giao thức TCP có tính chất công bằng (fairness) là nhờ chiến lược điều khiển tắc nghẽn theo kiểu Slow Start