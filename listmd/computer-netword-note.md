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
2. Thông lượng

### V. Các tầng giao thức, mô hình dịch vụ

## Application

### I. Tổng quan

### II. Nguyên tắc của netwwork applications
1. Giao tiếp giữa các tiến trình
2. Các mô hình app
3. Các yêu cầu của app

### III. Các giao thức phổ biến
1. Web và HTTP
2. FTP và truyền tệp
3. Electronic mail

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
