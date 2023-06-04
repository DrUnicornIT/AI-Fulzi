---
layout: page
title: Computer NetWork Note
permalink: courseuet/computer-network-note
---

## Introduction 

### I. The Internet
1. "Nuts and bolts" view
	- Hàng triệu thiết bị kết nối:
		- Host: Là người dùng cuối
		- Run các network app: Một ứng dụng nào đó được chạy
		- End users bao gồm: PC, Server, máy chủ, điện thoại, laptop, ...
	- Đường truyền kết nối: Communication links
		- Cáp đồng, cáp quang, radio, vệ tinh: không dây hoặc có dây
		- Đặc trưng: băng thông (band width): không phải tốc tộc truyền vật lý ~ độ lớn của đường ống truyền
	- Packet switches: chuyển tiếp gói tin (khối dữ liệu)
		- Bộ định tuyến (router)
		- Switches
	-  Internet: mạng của các mạng: Interconnected ISPs
	- Protocols: các giao thức (cách thức giao tiếp) của các mạng máy tính với nhau  điều kiển việc gửi, nhận các msg
	- Chuẩn Internet: RFC, IETF
2. Service view:
	- Cơ sở hạ tầng cung cấp dịch vụ cho các ứng dụng, Web, VoIP, Email, Games, ...
	- Cung cấp programming interface cho apps
3. Protocol: Định nghĩa format, thứ tự của các tin gửi, nhận giữa các thực thể mạng và những hành động được thực hiện khi truyền, nhận tin nhắn.

### II. Netwok edge: end-system, access networks, links 
1. Network structure
	- Network Edge:
		- Host: client và server
		- Máy chủ ở trung tâm dữ liệu
	- Access network, physical media: Đường truyền kết nối có dây, không dây
	- Network core: router, network of networks
2. Kết nối mạng và phương tiện vật lý
	- Thông số kết nối:
		- Băng thông kết nối (bits per secord): lượng dữ liệu truyền tối đa trong 1 đơn vị thời gian
		- Shared or dedicated?
		- Trễ (Latency): Thời gian tìm dữ liệu từ A->B
			- Trễ truyền tải: "kích thước dữ liệu / băng thông"
			- Trễ truyền dẫn: "độ dài liên kết / tốc độ tín hiệu"
3. Acces network
	- Access net
		- DSL: Đường dây thuê bao kĩ thuật số
		+ Cable network: Cáp mạng
			+ HFC: cáp quang, trục đồng: không đối xứng tới 30mbps downstream/ 2mbps upstream
			+ Network cable, cáp quang từ nhà to ISP router
	+ Enterprise access network (Ethernet)
		+ Mạng truy cập doanh nghiệp, thường dùng cho công ty, trường đại học
		+ 10mbps, 100, 1Gbps, 10Gbps
		+ Ngày nay, endsys thường kết nối Ethernet switch
	+ Không dây access network
		+ Dùng chung kết nối từ end sys -> router thông qua điểm truy cập
		+ Mạng không dây LANS
			+ Khoảng cách 100ft
			+ Wifi: 11,54 Mbps
		+ Mạng không dây khu vực rộng
			+ Cung cấp bởi nhà mạng điều hành viễn thông ~ 10 km
			+ Từ 1-> 10 Mbs
			+ 3G, 4G, LTE
4. Host (end system): Send packets of data
	-  Chức năng sending: 
		- Nhận message của app
		- Phá vỡ thành các gói nhỏ: Packet với độ dài L bits (bit)
		- Tên gói tin vào access network với tốc độ đường truyền là R (bit/sec)
			Tốc độ truyền link <=> link capacity <=> link bandwidth = R    
			Độ trễ truyền tin packet = thời gian cần để nén / gói tin dài L vào link = L/ R
5. Phương tiện vật lý: Băng tần, Tỉ lệ bỗi bit khi chuyền, Độ suy hao giảm tín hiệu khi truyền
	- bit
	- physical link: nằm giữa gửi và nhận
	- guided media: tín hiệu trìm trong phương tiện rắn: cáp quang, đồng, ...
	- unguided media, tín hiệu truyền tự do: radio
	- dây xoắn: twisted pair (TP): 2 dây đồng cách điện

### III. Network core
1. Network core
	- Lưới các routers kết nối với nhau
1. Packet-switching
	- Hosts bẻ vỡ app-layer mess thành các packets:
		- header: đại chỉ, số thứ tự
		- payload: phần dữ liệu
	- Chuyển tiếp gói tin từ 1 router sang 1 router tiếp theo
	- Mỗi gói được truyền tại với toàn bộ link capacity 
	+ Mất L/R s đẩy dữ liệu mỗi gói vào link
		+ store-and-forward: toàn bộ gói phải đếm được router trước khi được chuyển tiếp đi 
			=> End - end delay = 2L/R
	- Queueing delay, loss
		- Nếu tốc độ đến (in bits) link lớn hơn tốc độ truyền (in bits) của link trong một khoảng thời gian
			-> Các gói xếp hàng, chờ được trên trên link 
			-> Các gói bị mất khi queue đầy 
	- Two key network-core-functión
		- Routing: xác định tuyến đường đi của packet bằng thuật toán routing
		- Forwarding: chuyển gói tin từ router's input đến router's output chính xác
2. Circuit switching: chuyển tiếp data nhanh hơn
	- Mỗi link có n circuit (cố định thiết kế)
	- Tài nguyên phân bổ, duy trì dành riêng cho src và dst
	- Đoạn mạch nhàn rỗi nếu không được sử dụng
	- Thường sử dụng trong mạng điện thoại truyền thống
3. Packet switching vs Circuit switching
	- PS cho phép nhiều người dùng hơn sử dụng network
	- PS tốt cho dữ liệu nhanh:
		- Chia sẻ tài nguyên
		- Đơn giản, không thiết lập call
	- Những có thể xảy ra tắc nghẽn -> delay và mất gói tin
		-> Cần các giao thức để truyên tin tin cậy và điều khiển chống tắc nghẽn 
4. Internet Structure
	- End sys kết nối Internet thông qua ISPs: nhà cung cấp dịch vụ Internet ....
	- Access ISPs : p? được kết nối với nhau
	- Kết nối ISP -> global transit ISP
		- Các global ISP kết nối = IXP: Internet exchange point
		- Các mạng khu vực cũng có thể phát sinh và kết nối tới ISP

### IV. Delay, loss, thông lượng trong mạng
1. Trễ
	- d_proc: nodal processing
		- check bit lỗi 
		- xác định output link
		- thường < m sec
	- d_queue: trễ hàng đợi
		- đợi đến lượt vào link
		- thời gian thì phụ thuộc vào tốc độ tắc nghẽn
	- d_trans: thời gian đẩy vào link
		- L: packet length
		- R: link band width
		- d_trans = L/R
	- d_prop: độ trễ lan tràn
		- d: độ dài dây vật lý
		- s: tốc độ lan tràn
		- d_prop = d/s
		Tổng delay = d_prop + d_queue + d_trans + d_prop
2. Mất mát
	- Xảy ra khi hàng đợi đầy
	- Gói tin bị mất có thể được gửi lại từ node ngay lập tức, từ src end sys hoặc không
3. Thông lượng
	- (bit/time) tốc độ truyền giữa người gửi và người nhận
		- Tức thời: tại thời điểm cho trước
		- Trung bình: trên khoảng thời gian dài
	- = min(Ri) với Ri là băng thông của kết nối thành phần thứ i trên đường truyền

### V. Các tầng giao thức, mô hình dịch vụ
1. Mỗi layer implements 1 dịch vụ:
	- Thông qua những hành động bên trong của chính layer đó
	- Dựa vào các dịch vụ được cung cấp ở tầng dưới
2. Tại sao phải phân lớp? Giải quyết các hệ thống phức tạp
	-  Cấu trúc rõ ràng -> xác định mối quan hệ của hệ thống
	- Module hóa -> dễ bảo trì, cập nhật: thay đổi lớp này không ảnh hưởng lớp kia
3. Giao thức Internet: Hình đồng hồ cát
	- Application: hỗ trợ các ứng dụng mạng, đưa ra thông báo truyền tin. FTP, HTTP, SMTP
	- Transport: gửi dữ liệu giữa 2 tiến trình, đảm bảo chất lượng dịch vụ. TCP, UDP
	- Network: định tuyến datagrams từ src -> dst, đảm bảo chuyển đến địa chỉ nhận. IP, routing protocols
	- Link: Trên dữ liệu giữa 2 thiết bị, có kết nối vật lý trực tiếp. Ethernet, Wifi, PPP
	- Physical: chuyển bit -> tín hiệu (sóng điện từ, ....) và truyền
4. Mạng máy tính:
	- Tập các máy tính kết nối với nhau dựa trên một kiến trúc mạng nào đó để có thể trao đổi dữ liệu
5. Kiến trúc mạng:
	- Cách các nút mạng kết nối với nhau
		- Topology vật lý: hình trạng dựa trên cáp kết nối: bus, vòng, sao, lưới ...
		- Topology logic: hình trạng dựa trên cách thức truyền tín hiệu: điểm - điểm - điểm, điểm - đa điểm
	- Cách các nút mạng trao đổi dữ liệu với nhau (giao thức, protocol)
6. Phân loại mạng máy tính 
7. Kiến trúc Internet
	- Kết nối mỗi mạng -> mạng khu vực -> trạm chuyển tiếp của 1 nhà cung cấp toàn cầu
	- Các ISP kết nối với nhau qua IXP
8. Mô hình OSI/ISO
	- Giao diện (interface) định nghĩa cách thức và format dữ liệu trao đổi giữa 2 tầng liều nhau trong cùng một thiết bị
	- Tầng Datalink: truyền thông giữa 2 nút nối trực tiếp với nhau 
		- Đóng gói dữ liệu: chia luồn bit nhận được từ Network thành các frame
		- Định địa chỉ vật lý:
			- Cùng mạng: địa chỉ đích, địa chỉ nguồn
			- Khách mạng: địa chỉ nhận, địa chỉ thiết bị kết nối ra ngoài
		- Kiểm soát lưu lượng: khi tốc độ nhận < tốc độ gửi
		- Kiểm soát lỗi: 
			- Làm tăng tính tin cậy của tầng vật lý
			- Phát hiện, truyền lại các frame mất, xử lý trùng frame
		- Kiểm soát truy cập:
			- Giai đoạn thiết bị nào được dùng đường truyền chung tại một thời điểm
	- Tầng mạng (Network): chuyển gói dữ liệu từ nơi gửi -> nơi nhận, có thể phải qua nhiều chặng
		- Định đại chỉ logic -> tiêu đề gồm địa chỉ logic của thiết bị gửi, nhận
		- Định tuyến: các thiết bị kết nối trung gian (router, gateway) xác định tuyến đường để gói tin đến đích. 
		- Địa chỉ logic không đổi trong khi đi qua các mạng khác nhau
	- Tầng giao vận (Transport): Chuyển toàn bộ thông điệp từ nơi gửi -> nơi nhận. Đảm bảo gửi thông điệp một cách toàn vẹn. 
		- Đại chỉ cổng (port number): Header chứa địa chỉ tiến trình
		- Phân mảnh - tái hợp nhất: thông điểm -> nhiều segment nhỏ có số thứ tự cho phép ghép, kiểm tra đủ/thiếu
		- Kiểm soát kết nối: hướng nối - không hướng nối
		- Kiểm soát lưu lượng: gần giống tầng link nhưng giữa thiết bị đầu/cuối
		- Kiểm soát lỗi: giống tầng link nhưng thực hiện tại các thiết bị đầu/cuối
			-> đảm bảo toàn bộ thông điệp không lỗi (đủ, không hỏng, thừa)
	- Tầng phiên: thiết lập, duy trì và đồng bộ hóa tính liên tục 2 bên
	- Tầng tình diễn: biểu diễn cú pháp và ngữ nghĩa các thông tin được trao đổi giữa 2 hệ thống
	- Tầng ứng dụng: cho phpé người dùng truy cập, hỗ trợ các dịch vụ <gửi thư, quản lý csdl ...>
	- Chồng giao thức TCP/IP
	- Định danh trên TCP/IP
		- Tên miền
		- Port number
		- Địa chỉ IP
		- Địa chỉ vật lý/MAC
	- TCP/IP không có các cơ chế an toàn bảo mật thông tin

## Application

### I. Tổng quan
- Hoạt động trên các end systems, không hoạt động trên network-core
- Giao tiếp với nhau qua môi trường mạng
- Gồm 2 tiến trình:
	- Client: cung cấp giao diện NSD gửi thông điểm yêu cầu dịch vụ
	- Server: cung cấp dịch vụ, trả thông điệp đáp ứng

### II. Nguyên tắc của netwwork applications
1. Giao tiếp giữa các tiến trình
	- Tiến trình: chương trình đang chạy trong 1 host
		- Trong cùng 1 host, giao tiếp bằng inter-process communication
		- Khác host, giao tiếp bằng exchanging messages
	- Kiến trúc client-server
		- Client process: khởi tạo việc truyền dữ liệu, kết nối 
		- Server process: chờ client kết nối đến
	- Kiến trúc P2P có cả client process và server process
	- Socket (~hòm thư)
	- Định danh tiến trình: port number + 32-bit IP
	- Giao thức tầng app định nghĩa
		- Loại mgs: request, response
		- Syntax của mgs: có những trường nào, từng trường làm gì
		- Ngữ nghĩa của mgs: ý nghĩa của thông tin trong trường
		- Ruler: khi nào và như thế nào: tiến trình, đáp, gửi mgs
2. Các mô hình app
	- Client-server
		- Client:
			- Giao tiếp với server, không giao tiếp trực tiếp với máy khác khác
			- Có thể không liên lục kết nối
			- Có thể có địa chỉ IP động 
			- Gửi yêu cầu truy cập dịch vụ tới máy chủ
		- Server:
			- Luôn hoạt động chờ yêu cầu từ máy khách
			- Có địa chỉ IP cố định
			- Có thể có máy chủ dự phòng -> nâng cao hiệu năng, phòng sự cố
	- P2P
		- Không có máy chủ trung tâm luôn online
		- Các máy vai trò mang hàng, có thể giao tiếp trực tiếp với nhau
		- Các máy yêu cầu dịch vụ từ các máy khác -> tự mở rộng
		- Không kết nối thường xuyên, địa chỉ IP thay đổi -> quản lý phức tạp
		- Ưu điểm: 
			- Tự mở rộng do request tăng thì tài nguyên cũng tăng
			- Không cần chi phí cho server
		- Nhước điểm: 
			- Không biết chỗ nào lưu thứ mình cần -> phải đi tìm
	- Mô hình lai
		- Một máy chủ trung tâm để quản lý NSD, thông tin tìm kiếm, ...
		- Các máy khác giao tiếp trực tiếp với nhau sau khi đăng nhập
		- VD: Skype
3. Các yêu cầu của app
	- Toàn vẹn dữ liệu: đủ, đúng thứ tự, chính xác: một số yêu cầu 100%, một số cho phép loss
	- Thông lượng (real-time cần kích thước nhất định) (multi media)
	- Bảo mật: yêu cầu mã hóa ...
	- Tầng trans cung cấp 2 loại dịch vụ
		- TCP: truyền tin tin cập
			- Kiểm soát luồn: làm cho bên nhận không quá tải
			- Kiểm soát tắc nghẽn: tốc độ truyền của bên gửi sao cho mạng không quá tải
			- Không cung cấp: độ trễ, thông lượng tối thiểu, bảo mật
			- Hướng kết nối: (ảo, không phải vật lý): trước khi truyền phải thiết lập kết nối bên gửi - nhận
		- UDP: truyền tin không tin cậy
			- Không đảm bảo gì, không điều khiển
			- Không thiết lập kết nối
			-> Cần do xử lý nhanh gọn. Một số app không cần gì chỉ cần tốc độ (phát sóng trực tiếp ...)
		-> Cả 2 đều không có bảo mật -> tự thêm ở giữa (thư viện SSL thuộc tầng App) 
### III. Các giao thức phổ biến
1. Web và HTTP
	- Web
		- Web page gồm các đối tượng web: HTML file, ảnh, java applet, audio file, ...
		- Chứa các tham chiếu tới các đối tượng
		- Khi tải web pages sẽ tải các đối tượng và hiển thị lên (tải từ web server)
		- Các đối tượng địa chỉ = URL
			- Host name: tên miền IP server
			- Path name: đường dẫn đối tượng Web
	- HTTP: (hypertext transfer protocol)
		- Mô hình client - server
			- Client: trình duyệt web gửi 1 HTTP request đến server
			- Server: trả về 1 HTTP response (1 đối tượng web)
			- Client: nhận và "hiển thị" đối tượng web
		- Sử dụng dịch vụ TCP
			- Client thiết lập kết nối TCP (socket) tới server, cổng mặc định 80
			- Server chấp nhận kết nối từ client
			- Trao đổi qua lại, xong thì đống lại
		- Không trạng thái (state less): Các request xử lý độc lập, không quan tâm trước đó là gì
	- HTTP connection: 2 kiểu thiết lập kết nối
		- Non-persistent: kết nối không liên tục
			- Mỗi kết nối chỉ gửi nhận 1 đối tượng web
			- Xong thì đóng, tải tiếp lại tạo kết nối -> thời gian lớn
			- Quy trình: gửi yêu cầu kết nối, gửi request, tải file về
			=> Tổng time = 2RTT + thời gian tải file
		- Persistent: kết nối liên tục
			- Sau khi tải 1 file về vẫn duy trì đến khi tải xong
			- Nhược điểm: duy trì kết nới
				- Tăng tài, tài nguyên server 
				- Server giới hạn số lượng kết nối đồng thời
			- Non-persistent tiết kiệm tài nguyên hơn
	- HTTP message
		- HTTP request
			- Viết dưới dạng mã ASCII
			- Định dạng với GET
			- General format
			- Các pương thức Upload từ Input
				- POST: input chứa trong entity body
				- URL: như GET, input được tải lện trong URL ở request line
			- Các phương thức các phiên bản HTTP cung cấp
				- HTTP/1.0
				- HTTP/1.1
		- HTTP response
			- Định dạng: 
				- status line (protocol - status code - status phrase) trạng thái phiên bảo có thể khác lúc truy vấn
				- header lines
				- data
			- Một số code:
				- 200: Ok -> kèm data
				- 301: đối tượng yêu cầu đã di chuyển đến địa kiểm mới
				- 400: yêu cầu không hợp lệ -> yêu cầu không được hiểu bởi server
				- 404: không tìm thấy, không tìm thấy doc được yêu cầu
				- 505: Phiên bản HTTP không được hỗ trợ
	- Cookies:
		- Do HTTP không lưu trạng thái -> nếu dịch vụ Web cần xác thực thì xác thực với mội request
			-> server tạo ra mẩu dữ liệu và gửi cho client để mỗi lần request, client gửi thêm cái đó
		- 4 components:
			- Cookie header line của HTTP response mgs (từ server)
			- Cookie header line của HTTP request mgs (nhiều request của client)
			- Cookie file được lưu trữ trên host của người dùng, quản lý bởi browser của người dùng
			- Có cơ sở dữ liệu back-end ở Website
		- Cookie được sử dụng cho
			- Autorization: ủy quyền 
			- Giỏ hàng (trang web thương mại)
			- Recommendations
			- Trạng thái phiên (web email)
		- Cookie: chứa thông tin trạng thái của phiên, server có thể lưu lại cookie
	- Web cache: (proxy server)
		- Đáp ứng yêu cầu của người dùng mà không liên quan đến máy chủ gốc
		- Brower gửi tất cả HTTP requests cho cache
			- Nếu cache có: trả về đối tượng
			- Nếu cache không có: cache request đối tượng từ server gốc rồi trả cho client
		- Lợi ích
			- Giảm thời gian phản hồi cho client
			- Giảm áp lực đường truyền, lưu lượng truy cập trên access link 1 tổ chức
			- Giảm áp lực cho server
		- GET có kiều kiện, phòng trường hợp dữ liệu server thay đổi so với cache
2. FTP và truyền tệp
	- Tổng quan:
		- Truyền file từ máy chủ từ xa, cho phép cả tải về, tải lên
		- Mô hình client - server
			- Client: bên bắt đầu truyền (đến/từ xa)
			- Server host từ xa
		- Được tạo ra trước HTTP, đủ để gửi file, tin nhắn -> mong có ứng dụng chia sẻ hình ảnh, âm thành -> HTTP
		- FTP server: port 21
		- Sử dụng TCP tầng trans
	- Hoạt động
		- FTP client thiết lập kết nối TCP tới FTP server, cổng 21
		- Client phải đăng -> Client authorized trên kết nối điều khiển (control connection)
		- Client gửi lệnh qua control connection
		- Khi server nhận được lệnh, server thiết lập kết nối mới data connection cổng 20
			-> Server truyền data qua kết nối này, truyền xong ngắt data, không duy trì
			Khi nhận được lệnh tiếp, truyền data tiếp, server lại mở kết nối data connection
	- Lệnh và mã trả lời
		- Lệnh: ASCII text được gửi trên control channel:
			- USER, PASS, LIST, RETR (file name), STOK (file name)
		- Mã trả lời: status code - status phrase (như HTTP)
			- 331: UER name OK, yêu cầu pass
			- 125: data connection đã mở, bắt đầu truyền
			- 425: không thể mở data connection
			- 452: lỗi viết file
3. Electronic mail
	- Tổng quan
		- Gồm 3 thành phần chính 
			- Use agents
			- Mail servers
				- Main box
				- Message queue
			- SMTP protocol: giao thức gửi thư giữa các mail server
	- Mail server - giao thức SMTP (simple mail transfer protocol)
		- SMTP:
			- Tất cả các email đều dùng SMTP dùng rất cổ, script dài dòng
			- Dùng TCP cổng 25
			- Dùng tỏng pha từ 
				- client A -> server A
				- server A -> server B
			- Gửi trực tiếp không qua trung gian
			- 3 pha: bắt tay -> gửi -> đóng
			- Tương tác
				- Lệnh ASCII text
				- Trả lời: status code and phrase
			-  Kết nối liên tục, duy trì đến khi hết phiên
		- So sánh với HTTP:
			- HTTP: kéo, 1 đối tượng trong 1 msg
			- SMTP: đẩy nhiều đối tượng trong 1 msg
		- Mail msg format:
			- SMTP: yêu cầu msg (cả header và body) là 7-bit ÁCII
	- Giao thức nhận thư (mail access)
		- POP/IMAP
		- POP
		- POP3 (Post office protocol)
		- IMAP (Internet Mail Acces Protocol)
		- Nếu dùng HTTP: mỗi click vẫn chỉ lấy được 1 obj (mở ảnh .. cần request khác)
### IV. DNS
1. Tổng quan
2. Dịch vụ DNS
3. Cấu trúc DNS
4. Cơ chế truy vấn của DNS
5. Cache của local DNS
6. DNS records
7. DNS protocol, MSG

#### Các dạng bài tập
1. Truy cập vào web
2. Thời gian tải đối tượng web
3. File distribution

## Transport Layer

### I. Tổng quan

### II. Dồn kênh, phân loại kênh

### III. UDP - User Datagram Protocol

### IV. Các dịch vụ khác và TCP
1. Truyền tin tin cậy
2. TCP
3. Điều khiển tắc nghẽn

### V. Fairness

## Network layer

### I. Giới thiệu 

### II. Các dịch vụ kết nối

### III. Cấu trúc router

### IV. IP - Internet Protocol 
1. IP datagram format
2. IP v4 address
3. Giao thức ICMP (Internet Control Message Protocol)
4. IP v6

### V. Các thuật toán định tuyến
1. Link state
2. Distance vector
3. Định tuyến phân cấp

### VI. Định tuyến trên mạng Internet
1. Định tuyến nội miền AS
2. Định tuyến liên miền BGD - Border Gateway Protocol

#### Bài tập ví dụ

## Link layer

### I. Tổng quan

### II. Phát hiện lỗi - sử lỗi

### III.  Multiple access protocol 

1. TDMA: Time division multiple access
2. FDMA: Frequency ...
3. Random access 
4. "Tacking turn" MAC protocol

### IV. LANS
1. MAC add và ARP
2. Ethernet
3. Hubs - swiches: thiết bị phần cứng
4. VLANS
