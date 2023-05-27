---
layout: page
title: Software Engineering
permalink: courseuet/software-engineering
---

## Các khái niệm cơ bản về Công Nghệ Phần Mềm

### I. Sản phẩm phần mềm

Là sản phẩm của quá trình phát triển phần mềm (bao gồm cả làm dữ liệu)   
Cần hiểu đúng để nhận bàn giao đủ, tránh khó khăn trong việc chỉnh sửa về sau   
Khách hàng có thể thuê đơn vị giám sát (xem hiểu các tài liệu, các phần) để nhận bàn giao   
- Khái niệm phần mềm gồm:
	- Component Program: tập các câu lệnh có 2 mức độ mã nguồn (source code) và mã máy (executable) đã compile khác nhau tùy mô trường. Khi được thực hiện sẽ tạo ra các dịch vụ và đem lại các kết quả mong muốn cho users. 
	- Data Structure: ngoài (database) thiết kế database phải mở rộng được (lưu trữ), (RAM) cấu trúc dữ liệu sử dụng trong code (làm việc) làm cho chương trình thao tác hiệu quả với các thông tin thích hợp (thông tin -> số hóa)
	- Document: Tài liệu kỹ thuật: kế hoạch triển khai, đặc tả, thiết kế chi tiết code, test); HDSD/Đào tạo: được yêu cầu trong pháp lý, mô tả thao tác, cách sử dụng và bảo quản phần mềm

- Tầm quan trọng của phần mềm (vai trò)
	- Nền Kinh tế các quốc gia phụ thuộc và phần mềm: thu chi từ phần mềm, tổn thất do phần mềm sai/hỏng   
	- Phần mềm tạo ra sự khác biệt trong tổ chức: phong cách làm việc, năng suất lao động, thương hiệu   
	- Con người ngày càng phụ thuộc vào phần mềm   
	- Xu hướng: tin học hóa toàn bộ các hoạt động của hầu hết các lĩnh vực   
Ví dụ như: Amazon, Walmart   

### II. Các đặc trưng của phần mềm  

Phần mềm là phần tử hệ thống logic, không phải hệ thống vật lý   
1. Không mòn cũ hỏng như Hardware (tuổi thọ của thiết bị, va đập, độ ẩm, môi trường ..) nhưng thoái hóa theo thời gian. Có 3 nguyên nhân khiến phần mềm cũ (thoái hóa) “hỏng”:
	+ Lỗi phát sinh khi đang dùng (do chưa test phát hiện)
	+  Môi trường thay đổi: Phần cứng: máy móc thiết bị, mạng, máy chủ; Phần mềm: hệ điều hành, các tiện ích (import)
	+ Nhu cầu thay đổi nghiệp vụ (phát sinh tính năng mới, chỉnh sửa tính năng cũ đáp ứng nhu cầu mới). Lỗi do nâng cấp, trước khi đi về tỉ lệ ổn định thì lại phải yêu cầu thay đổi -> phát sinh đỉnh nhọn tiếp theo -> mức tối thiểu tăng dần. Ván sửa nhiều đến lúc không thể sửa được nữa.
2. Không được ráp từ mẫu có sẵn:
	- Không có danh mục chi tiết cho trước: không được định hướng trước, phát triển xong mới biết hoạt động có hiệu quả hay không?
	- Sản phẩm đặt hàng theo yêu cầu riêng: “máy đo": 1 khách hàng + 1 cty -> 1SP. Theo đơn vị hoàn chỉnh phụ thuộc vào yêu cầu riêng của khách hàng. Ít khi có thể lắp ráp theo khuôn mẫu có sẵn như hardware. Sản phẩm dùng chung phải nghiên cứu nhu cầu thị trường.
3. Phức tạp, khó hiểu, vô hình:
	- Là những khái niệm được thể hiện bằng 1 hệ thống logic thông qua nhận thức khái niệm và quá trình tư duy trừu tượng.
	- Không thể nhìn thấy được -> nhận biết qua sự mô tả của các khía cạnh khác nhau (sơ đồ điều khiển, sơ đồ luồng dữ liệu …)
4. Luôn luôn thay đổi:
	- Nghiệp vụ thay đổi
	- Nhu cầu con người thay đổi
	- Môi trường vận hành thay đổi 
	- Lỗi phát sinh (do đảm bảo chất lượng phần mềm chưa tốt). Phần mềm là mô hình của thế giới thực. Thế giới thực luôn thay đổi theo không gian và thời gian -> Phần mềm chỉ có ý nghĩa khi thích nghi được với những thay đổi diễn ra, thay đổi trở thành yêu cầu và thuộc tính tất yếu của phần mềm
5. Cần phát triển theo nhóm:
	-  Yêu cầu những kỹ năng khác nhau (Năng lực của nhóm sẽ tuyến tính với số người. Thời gian trao đổi thông tin chiếm tỉ lệ cao
	- Nhu cầu bàn giao nhanh
    
### III. Information System

IS bao gồm: Hardware, Network communication, SW, Data, Đào tạo người dùng (đặc biệt về an ninh an toàn), Business process (chiến lược, nghiệp vụ -> kỹ thuật quy trình nghiệp vụ phải thay đổi dẫn tới -> 1 quy trình phù hợp chuẩn hóa quy trình)

### IV. Phân loại    
Có nhiều cách phân loại phần mềm, 1 phần mềm có thể thuộc nhiều loại   
Thường chia theo chức năng
	- Phần mềm hệ thống (system software) điều hành hoạt động máy tính, thiết bị, chương trình (hệ điều hành), trợ giúp các tiết tích (tổ chức tệp, nén, dọn dữ liệu)
	- Phần mềm nghiệp vụ: Trợ giúp các hoạt động nghiệp vụ khác nhau, phân làm 2 loại là sản phẩm đặt hàng và sản phẩm chung
	- Phần mềm công cụ (Case tools): Computer Aided SE Trợ giúp quá trình tạo ra các phần mềm: gồm công cụ trợ giúp quá trình phát triển phần mềm bằng máy tính, các ngôn ngữ lập trình (trình soạn thảo, trình soát lỗi, chương trình dịch, thư viện …). Hỗ trợ tự động hoá một số pha/ bước trong quy trình phát triển PM 
	    
### V. Các tiêu chí của phần mềm    

1. Với các bên liên quan:
	- Chủ đầu tư (người trả tiền): chi phí phát triển phù hợp, thời gian ngắn 9nhanh mang lại lợi nhuận), dễ bảo trì
	- Người dùng: đủ chức năng/ nghiệp vụ, dễ sử dụng, tin cậy, an toàn, thông minh
	- Nhà phát triển (từ lãnh đạo -> chuyên viên) sản phẩm chất lượng cao (khẳng định năng lực, quảng bá), dễ bảo trì
2. Mô hình chất lượng cho chất lượng:
	- Tính năng: phù hợp, chính xác, an toàn, dễ tương tác
	- Tính tin cậy: hoàn thiện, khả năng chịu lỗi, khả năng phục hồi
	- Tính khả dụng: dễ hiểu, dễ học, khả năng vận hành, tính hấp dẫn
	- Tính hiệu quả: Đáp ứng thời gian sử dụng tai nguyên
	- Khả năng bảo trì: Khả năng phân tích, khả năng thay đổi, tính cân bằng, khả năng khẳng định
	- Tính khả chuyển: Khả năng thương hợp, khả năng cài đặt, khả năng chung sống, khả năng thay thế
3. Tổng quan:
	- Có chuẩn để có thể liên kết rộng rãi
	- Trong hợp đồng sản phẩm phải ghi rõ theo tiêu chuẩn chất lượng gì: cái gì, do như thế nào, đạt tiêu chuẩn gì
	- Trong thực tế chỉ chọn quan tâm một số tiêu chuẩn cụ thể
	- Trong làm và tự đánh giá: bản thân phải có chuẩn, công ty đã cam kết với xã hội làm chuẩn nào, tiêu chí của công ty đưa ra …
4. Tính năng
	- Tính phù hợp: phù hợp với nghiệp vụ:
		- Là khả năng có thể cung cấp 1 tập các chức năng thích hợp cho công việc cụ thể phục vụ mục đích của người sử dụng
		- Để đo được thì chọn <ngẫu nhiên có phân hoạch> người sử dụng, nếu trên một ngưỡng (đã thống nhất) thấy phù hợp thì OK -> Sự chấp nhận của người dùng về phù hợp của tính năng
	- Tính chính xác:
		- Có thể cung cấp các kết quả hay hiệu quả đúng đắn hoặc chấp nhận được với độ chính xác cần thiết
		- Cách đo như trên. Về quy trình có phản ánh đúng quy trình nghiệp vụ không, output có chính xác không (test input -> output có chuẩn không …)
	- Khả năng hợp tác (phụ):
		- Tương tác với 1 số hệ thống cụ thể khác, “nói chuyện” được với phần mềm khác trong hệ thống hoặc với các hệ thống trong cùng 1 công ty? Tùy vào database của các phần mềm khác (được cấp phép ntn) ?
	- Tính an toàn (quan trọng):
		- Khả năng bảo vệ thông tin và dữ liệu của sản phẩm phần mềm sao cho người, hệ thống không được phép thì không thể truy cập, đọc hay chỉnh sửa chúng
		- VD: đề ra quy chuẩn bách up dữ liệu ntn cho máy chủ (về vật lý), mô phỏng sự tấn công xem phần mềm có chịu được không (về logic)
	- Độ tin cậy:
		- Tính hoàn thiện (Khó): Khả năng tránh các kết quả sai, áp dụng các kỹ thuật cao cấp, phân tích mã nguồn -> lỗi tiềm năng, công cụ toán học -> chứng minh không có lỗi
		- Khả năng chịu lỗi: Khả năng hoạt động ổn định tại một mức nào đố kể cả có lỗi xảy ra.
		- Khả năng phục hồi: Có thể tái thiết lại hoạt động tại một mức xác định và khôi phục dữ liệu liên quan trực tiếp đế lỗi, Đo thời gian trung bình để xử lý lỗi (khi có lỗi -> recover), quy định về thời gian tối đa
	- Tính khả dụng: đa số dùng khảo sát cảm nhật chủ quan của người dùng
		-  Dễ hiểu: người dùng có thể hiểu được xem PM có phù hợp với họ không và sử dụng thế nào cho những công việc cụ thể
		-  Dễ học. 
		-  Có thể sử dụng được
		-  Tính hấp dẫn
	- Tính hiệu quả: có công cụ test
		- Đáp ứng thời gian: Khả năng đưa ra kết quả, 1 thời gian xử lý vào 1 tốc độ đo thông lượng hợp lý khi nó thực hiện công việc của mình dưới 1 điều kiện làm việc xác định (thời gian phản hồi, khả năng chịu tải)
		- Sử dụng tài nguyên: khả năng của phần mềm  có thể sử dụng 1 lượng, 1 loại tài nguyên hợp lý để thực hiện công việc trong những điều kiện cụ thể
	-  Dễ bảo trì: Tài liệu đầy đủ, kiến trúc hệ thống linh hoạt
		- Có thể phân tích được: có thể được chẩn đoán để truy tìm những thiếu sót hay những nguyên nhân gây lỗi hoặc để xác định những phần cần sửa
		- Có thể thay đổi được có thể chấp nhận một số thay đổi cụ thể trong quá trình triển khai
		- Tính ổn định: khả năng tránh các tác động không mong muốn khi chính sửa phần mềm
		- Có thể kiểm tra được: khả năng cho phép đánh giá được phần mềm chỉnh sửa
	- Tính khả chuyển:
		- Khả năng thích nghi có thể thích nghi với nhiều môi trường khác nhau mà không cần thay đổi
		- Có thể cài đặt được phần mềm có thể cài đặt được trên những môi trường cụ thể
		- Khả năng cùng tồn tại: có thể cùng tồn tại với những phần mềm độc lập khác trong một môi trường chung, cùng chia sẻ tài nguyên chung
		- Khả năng thay thế: có thể dùng thay thế cho một phần mềm khác với cùng mục đích và trong cùng môi trường

### VI. Tiến hóa phần mềm và thách thức

1. Sự thay đổi của phần mềm:
	- Thay đổi là bản chất của phần mềm
	- Phần mềm thay đổi khi Lỗi phát sinh, 1 yêu cầu cũ bị sửa hoặc bị loại bỏ, 1 yêu cầu mới phát sinh, môi trường phần mềm thay đổi. (Cái nào trong giai đoạn phát triển, cái nào trong giai đoạn vận hành)
2. Nguyên nhân thay đổi:
	- Đảm bảo chất lượng có vấn đề 
	- Quá trình thu thập, phân tích và đặc tả yêu cầu có vấn đề (thời gian ép, làm ẩu, khách hàng không hợp tác)
	- Nhu cầu con người ngày càng cao và phức tạp
	- Nghiệp vụ của các tổ chức cũng thường xuyên thay đổi, tái cấu trúc
	- Môi trường phần mềm thường xuyên thay đổi
3. Thách thức đặt ra:
	- Tăng chi phí cho quá trình phát triển (re-work)
	- Tăng chi phí cho doanh nghiệp trong quá trình bảo trì (chi phí bảo trì >> phát triển)
	- Phát sinh nhiều vấn đề lớn (kỹ thuật, ứng dụng)
	    

## Software Engineering



### I. Khái niệm về SE

1. Mục tiêu của SE:
	- Làm thế nào để có được sản phẩm phần mềm có chất lượng cao (đủ tính năng, dễ dùng) thời gian phát triển ngắn, chi phí phát triển “thấp" trong môi trường đầy biến động, thay đổi (chưa đạt được mục tiêu)
	- Về mặt vĩ mô:  
		- SE là 1 ngành công nghiệp, là 1 ngành của các nền kinh tế, liên quan đến mọi khía cạnh của việc phát triển phần mềm (thu thập, phân tích và đặc tả, thiết kế, lập trình, kiểm thử, chuyển giao, vận hành và bảo trì…)
		- Gồm 2 phần (2 lĩnh vực)
			- Hàn lâm (việc nghiên cứu, trường đại học): nghiên cứu, đề xuất các giải pháp cho các vấn đề mà công nghiệp đặt ra
			- Công nghiệp: phát triển, chuyển giao phần mềm
			- R&D: mảng việc chung (giao) của 2 đối tượng trên là R&D&C
		- Ngành công nghiệp mạnh khi cả 2 phần cùng mạnh:	  
			- Các nhà khoa học: đề xuất các giải pháp, các phương pháp và công cụ, có thời gian “vô hạn"   
			- Các kỹ sư PM: Phát triển 1 giải pháp cho 1 vấn đề cụ thể với 1 khách hàng cụ thể, sử dụng ngôn ngữ, công cụ, kỹ thuật cụ thể, phương pháp cụ thể, làm việc trong nhiều miền ứng dụng khác nhau, có thời hạn làm việc nghiêm ngặt, cụ thể. Luôn đối mặt với môi trường đầy biến động (thay đổi)   
		- Về nội hàm (khái niệm SE)
			- Bao gồm các nguyên lý, chiến lược (có nhiều và phù hợp với từng loại Phần Mềm) dưới mỗi chiến lược gồm rất nhiều phương pháp mô hình < phương pháp có thể được hiểu là cách làm cụ thể để phát triển PM đạt được mục tiêu trên> với mỗi mô hình phương pháp cách làm đó gồm các giai đoạn, các pha
			- Tương ứng với từng giai đoạn/ pha có các kỹ thuật và công cụ hỗ trợ, các kỹ năng kèm theo của người phát triển ra phần mềm đấy. 
			- Các công cụ hỗ trợ tự động, bán tự động, Công cụ được công ty setup sẵn và nhân viên được training
		- Yếu tố cơ bản của SE có thủ tục, phương pháp và công cụ. 
			- Thủ tục quy trình quản lý và phát triển là chất thứ giúp các phương pháp và công cụ gắn kết lại với nhau, làm cho chúng được sử dụng hợp lý đúng đắn

### II. Vòng đời phát triển của Phần Mềm

Là các hoạt động từ khi được đặt hàng, phát triển, sử dụng đến khi loại bỏ nó. Một hợp đồng chỉ cover gđ phát triển, chỉ ký cam kết bảo trì. Công ty phải có trách nhiệm trọn đời với sản phẩm mình làm ra.    
Về pháp lý: theo hợp đồng bảo hành theo điều khoản kết hợp với đạo đức nghề nghiệp. Khi có yêu cầu mới -> hợp đồng mới   

### III. Thách thức trong quá trình phát triển PM

- Hiện tại vẫn chưa có giải pháp đủ tốt, đặc biệt là với các phần mềm quy mô lớn. Phát triển ứng dụng lớn là 1 trong những công việc khó nhất -> nhiều rủi ro và thách thức
- 3 tiêu chí dẫn đến dự án thất bại:    
	- Không đạt được chức năng cam kết (implement và dễ dùng)
	- Vượt quá kinh phí
	- Vượt quá thời gian
 -> Thực trạng các dự án ở VN: nhỏ lẻ, manh mún, thiếu thiết kế tổng thể, chất lượng thấp, khó/ không thể năng cấp, bảo trì
 
### IV. Chi phí

- Khi phát triển 1 hệ thống thông tin, chi phí phần cứng không đáng kể so với phần mềm
- Trong phần mềm: 
	- Chi phí phát triển: 1/3 khách hàng + 1/6 lập trình + 1/2 kiểm thử
	- Chi phí bảo trì: Lớn hơn rất nhiều so với phát triển  
    
### V. Đạo đức nghề nghiệp

Tự thực hiện là chính, quan trọng nhất là pháp luật, quy định công ty.   
Về cơ bản thật thà, trung thực, cố gắng, không có tình làm sai, không chia sẻ sai người   
Khi cần thiết thì quản lý sẽ chỉ cho nên ưu tiên cái nào hơn cái nào hơn   
Vi phạm quy chế chắc chắn vi phạm đạo đức.   

## Software Process

### I. Software development process

- Mỗi mô hình được hình thành từ tổng hợp thực tiễn trong quá trình phát triển Phần Mềm. Nó là cách làm điển hình, hay, hiệu quả với 1 lớp dự án cụ thể, 1 tập các sản phẩm có đặc thù riêng
- Không có mô hình đủ tốt cho mọi sản phẩm
- Mô hình gồm các pha (giai đoạn) để phát triển Phần Mềm hiệu quả. Các mô hình thường khác nhau ở thứ tự thực hiện, cách triển khai công việc trong từng các pha.
- Tiến trình: là tập hợp các hoạt động để tạo ra Phần Mềm
    
### II. Mô hình thác nước
1. Tổng quan - ý tưởng chính:
	- Là mô hình đầu tiên, kinh điểm, định nghĩa các pha của quá trình phát triển phần mềm. Phân tách các giai đoạn đặc tả và phát triển, hệ thống, tuần tự, chặt chẽ
	- Các pha được thực hiện tuần tự. Xong hoàn toàn pha trước mới đến pha sau.
	- Được phép quay lại tại bất cứ pha nào, thời điểm nào nhưng phải đảm bảo tính tuần tự. Quay lại phải dừng ngay pha đang làm -> quay lại rồi sửa từ pha đó trở đi. -> Bùng nổ công việc khi quay lại ở các pha cuối
2. Ưu điểm  
	- Đơn giản, dễ hiểu, dễ dùng (do tiến hành tuần tự, công việc tiếp diễn đơn giản)
	- Cung cấp cấu trúc cho nhân viên chưa có kinh nghiệm (dễ apply, dễ học, chưa cần nhiều biện pháp phức tạp)
	- Các yêu cầu rõ ràng: yêu cầu được xác định từ đầu, cố định
	- Dễ hiểu, xác định được các mốc quan trọng của dự án
	- Dễ quản lý
	- Có khả năng đảm bảo chất lượng cho sản phẩm chất lượng cao:
		- Thỏa mãn tốt những yêu cầu khách hàng đặt ra, nhận thức được bất lợi to lớn, nếu phải quay lại muộn -> thái độ làm việc nghiêm túc, cẩn trọng, hiệu quả tốt
		- Dễ bảo trì: tài liệu đầy đủ và dễ chỉnh sửa tài liệu (tài liệu từng pha được hoàn thành đầy đủ từng pha gói gọn. Khi quay lại sửa đồng thời)
3. Nhược điểm 
	- Khó đáp ứng khi khách hàng thay đổi yêu cầu
		- Cố định các yêu cầu, rõ ràng ngay từ đầu: khó do phát sinh chỉnh sửa theo nhu cầu của khách hàng <hiểu lầm, phát biểu sai …>
		- Không linh hoạt, vỡ trận nếu sửa ở pha cuối (ảnh hưởng tới tiến độ)
	- Chậm có phiên bản thực hiện được: đến tận cuối mới được demo
		- Sai sót phát hiện muộn -> tổn thất lớn
		- Tâm lý khách hàng: mất kiên nhẫn -> gây sức ép, mất lòng tin
		- Khách hàng không đủ thời gian đưa ra comment
		- Ít thời gian đào tạo khách hàng, kết quả đào tạo sử dụng thấp -> Khách hàng gây ra lỗi và tin là do bên phát triển (50% lỗi là do người dùng chưa thành thạo)
	- Thời gian, chi phí, công sức bỏ ra lớn: thời gian dài
	- Test chung chung và muộn
4. Những tình huống sử dụng phù hợp
	- Các sản phẩm vừa và nhỏ, dự án ngắn hạn
	- Các sản phẩm yêu cầu chất lượng cao
	- Các sản phẩm có yêu cầu rõ ràng ngay từ đầu, không thay đổi (VD: tạo ra phiên bản mới của sản phẩm có sẵn, chuyển sản phẩm có sẵn sang nền tảng mới)
		-> Rủi ro cao với những hệ thống mới

### III. Mô hình chữ V

1. Tổng quan
- Bản chất là cải tiến của thác nước -> sự tuần tự
- Vấn đề cải tiến: kiểm thử ở thác nước diễn ra chung chung và tiến hành quá muộn. Kiểm thử có 2 bước: sinh bộ test và chạy bộ test
- Cải tiến như thế nào?:
	- Pha phân tích và đặc tả yêu cầu:
		Làm việc như cũ + sinh test kiểm thử chấp nhận -> khi sản phẩm passed tất cả các tests -> sản phẩm đáp ứng yêu cầu của khách hàng
	- Pha thiết kế:
		Thiết kế kiến trúc + sinh test kiểm thử tích hợp -> các module có tương tác được với nhau
		Thiết kế chi tiết + unit test -> test theo từng unit -> pass -> thích hợp
		-> Test đảm bảo thành phần đó đúng với thiết kế
	=> 
		Ở mỗi pha đều thêm vào khâu sinh bộ test phục vụ chạy test sau này
		Ở pha kiểm thử là lúc chạy lần lượt -> sai quay lại sửa 
		-> Kiểm thử có kế hoạch sớm, sinh ra độc lập khách quan với cài đặt
		-> kiểm thử mịn hơn
2. Ưu, nhược điểm - ứng dụng: như thác nước trừ phần cải tiến 

### Mô hình bản mẫu

1. Tổng quan - ý tưởng
	- Giải quyết bài toán của thác nước là làm rõ yêu cầu khách hàng từ đầu.
	- Các bước thực hiện:
		- Khảo sát sơ bộ để có được yêu cầu sơ bộ (2 bên gặp nhau, xác định mục tiêu tổng thể của phần mềm, xác định yêu cầu đặc biệt, các miền cần khảo sát thêm)
		- Thiết kế nhanh bản mẫu (trực quan hóa = bản vẽ, tool, giao diện giả click vào ra gì, ra gì …)
		- Hỏi ý kiến của khách hàng (khách hàng góp ý phản hồi, khách hàng sẽ cf với những yêu cầu chưa rõ ràng)
		- Chỉnh sửa bản mẫu theo feedback
		-> Bản mẫu cuối cùng khách hàng (ok)
		-> Coi như hiểu rõ yêu cầu chính xác -> áp dụng quy trình: phát triển SP, kiểm thử…
2. Ưu điểm
	- Giải quyết được những yêu cầu không rõ ràng, thông qua bản mẫu hiểu được yêu cầu chính xác hơn.
	- Giảm thời gian và chi phí tổng quan: do xác định sớm những gì người dùng thực sự muốn (chấp nhận thay đổi)
	- Cải thiện, gia tăng sự tham gia của người dùng:
		- Nhận được nhiều cmt từ khách hàng (yêu cầu, thông số .. ) đầy đủ chính xác, tiết lộ hiểu lầm …
			-> sản phẩm cuối cùng chính xác hơn, dễ dự trù phát sinh.
		- Giảm bớt gánh nặng đào tạo, chuyển giao do khách hàng tiếp xúc sớm, dễ làm chủ
			-> Tăng độ thỏa mãn, ít nóng ruột của khách hàng do sớm thấy bóng dáng sản phẩm trong bản mẫu sớm có phiên bản dùng được cho khách hàng
3. Nhược điểm
	- Chi phí làm bản mẫu lớn (cần nhân lực để làm chuyện này)
	- Mất nhiều thời gian cho thiết kế bản mẫu, đặc tả -> thời gian cho các pha khác hạn chế chất lượng mã nguồn có vấn đề, khả năng thay đổi có vấn đề
	- Yêu cầu khách hàng tham gia như một thành viên của dự án là rất khó, tốn thời gian tương tác, khó cho khách hàng, có thể sa đà tranh luận bản mẫu.
4. Ứng dụng
	- Các hệ thống vừa và nhỏ đặc biệt khi yêu cầu chưa rõ ràng, chưa xác định cụ thể input, output, chưa chắc chắn nội dung xử lý hay hiệu quả một thuật toán 
	- Ít được dùng như một hình phát triển cho một sản phẩm hoàn 
		-> dùng như một kỹ thuật cải tiến mô hình khác trong thu thập đặc tả yêu cầu 

### V. Mô hình xoắn ốc

1. Tổng quan ý tưởng:
	- Xoắn ốc = thác nước + bản mẫu + phân tích rủi ro
	- Giải quyết cho hạn chế của thác nước: được dành cho các sản phẩm lớn, phức tạp. Do làm việc rủi ro cao hơn, thiệt hại lớn hơn nếu fail
	- Để phát triển sản phẩm lớn:
		- Lập danh sách các yêu cầu (có sự đánh gái, trọng số, phân ưu tiên trong yếu) xử lý core -> mở rộng ra medium -> phần phụ
		- Lập kế hoạch phần core: xác định mục tiêu (chức năng, hiệu suất…), các ràng buộc (chi phí, thời gian, giao diện), các phương án thay thế (tái sử dụng, mua, …)
		- Phân tích rủi ro (quyết định làm/không làm): Xác định rủi ro (kinh nghiệm, công nghệ, lịch trình…), nghiên cứu các lựa chọn thay thế, giải pháp xử lý rủi ro -> tư vấn khách hàng, đề xuất khách hàng
		- Tiến hành làm bản mẫu, thực thi kĩ thuật: thiết kế, đánh giá thiết kế, phát triển mã, kiểm thử …
		- Đánh giá, hỏi ý kiến khách hàng -> sửa đổi -> lập lại cho đến khi xong core
		- Tương tự với các phần medium, phụ …
	- Cách tiếp cận tăng tiến: lặp tăng dần
	- Tư tưởng rất lớn hay -> Agile, RUP có bóng dáng xoắn ốc rõ
2. Ưu điểm: 
	- Cung cấp dấu hiệu sớm về việc không thể vượt quá rủi ro (do có phân tích rủi ro) tiết kiệm thời gian công sức.
	- Người dùng thấy hệ thống sớm (vì có bản mẫu sớm)
	- Các chức năng quan trọng được phát triển đầu tiên
	- Phản hồi sớm và thường xuyên từ người dùng 
	- Sản phẩm được làm theo từng phần dễ kiểm soát
3. Nhược điểm:
	- Cần có chuyên gia đánh giá rủi ro, chi phí cho pha này tốn kém
	- Xoắn ốc có thể vô thời hạn do yêu cầu thay đổi thường xuyên
	- Quy trình phát triển dài, phức tạp, quay vòng linh hoạt -> quản lý khó khăn
4. Ứng dụng:
	- Khi đánh giá chi phí và rủi ro là quan trọng
	- Dự án có quy mô lớn, yêu cầu phức tạp, đủ chi phí đầu tư

### VI. Component-based SW development (CBSD)

Là một mô hình của chiến lược Reuse-Oriented (phần mềm tái sử dụng và định hướng)  
1. Ý tưởng chính: 
	Hướng đến phát triển các ứng dụng lớn với CLC bằng cách sử dụng lại các thành phần phần mềm đã được phát triển trước đây (và đã được vận hành trong các hệ thống hiện đại)
2. Thành phần phần mềm:
	- Là một đơn vị phần mềm (gói-package hoặc module) đóng gói một tập các dịch vụ có liên quan (dịch vụ dùng chung dữ liệu, cùng miền quy trình nghiệp vụ
	- Một thành phần đều có tên (name), giao diện (interface) và mã (code)
3. Hình thức:
	Vẫn đặc tả, phân tích, thiết kế … nhưng một phần des là hầu hết cài đặt là kết hợp từ các thành phần có sẵn
4. Các bước:
	- Đặc tả yêu cầu
	- Phân tích thành phần - phân tích yêu cầu nào ứng với thành phần nào
	- Sửa đổi yêu cần
	- Thiết kế hệ thống với sử dụng lại
	- Phát triển và tích hợp - vấn đề bảo trì lỗi xảy ra ở việc tích hợp, ghép lại
	- Thẩm định sản phẩm

-> Là một trong những mô hình đảm bảo chất lượng rất cao do chất lượng các component đã được đảm bảo và linh hoạt trong thay đổi

### VII. RUP - Rational Unified Process

Hay sử dụng cho các dự án lớn      
Xây dựng công nghệ thông tin cho chính phủ thường chỉ định RUP   
Gắn liền với phát triển hướng đối tượng, UML   

RUP = thác nước + tiến hóa + sử dụng lại thành phần   
Thác nước: trong mỗi vòng lặp thực hiện xong workflows trên mới đến workflows dưới theo thứ tự tuần tự   
Tiến hóa: Phát triển phần mềm từ các yêu cầu ở core (ở các chu kì đầu) cho đến các yêu cầu có độ ưu tiên thấp hơn   
Sử dụng lại thành phần: Cấu trúc hệ thống thành các phần con để có thể sử dụng lại    

- Khía cạnh động của RUP được thể hiện qua 4 pha:
	Inception -> Elaboration -> Construction -> Transition
- Nguyên lý hoạt động:
	(thác nước, mỗi pha thực hiện các hđ tương ứng) khác mỗi pha trong RUP thực hiện hết các workflows và lặp lại quá trình đó
	Sự lập theo 2 cách: lặp các workflows trong mỗi pha, lập lại các pha (ở mỗi chu kỳ đi qua 4 pha)
	-> Sự lặp lại cho phép xác định từng bước các thành phần -> thành phần nào có thể sử dụng lại

### VIII. RAD - Rapid development

- Mục tiêu là phát triển các ứng dụng lớn
- Chia 1 dự án thành nhiều dự án con riêng chia cho nhiều teams và dùng thác nước ở mỗi team

### IX. TDD- Test driver development

- Không triển khai tuần tự
- Viết đặc tả yêu cầu bằng user stories và chuyển thành test scripts. Viết test trước, phát triển sau và chạy test scripts cho pass thì thôi

### X. Agile method

1. Agile: 
	Không phải là mô hình phát triển phần mềm mà là một phương pháp, cách tiếp cận, chiến lược: tập các nguyên tắc thực hành cho phát triển Phần Mềm. Những cái hiện thực hóa chiến lược là các phương pháp phát triển của Phần mềm: Scrum, XP
2. Khung cảnh ra đời: 
	Các yêu cầu ban đầu chắc chắn thay đổi, phần mềm mới cần được phát triển nhanh để đáp ứng các cơ hội
3. Agile Methods:
	- Phát triển tăng dần
	- Phiên bản mới được làm trong 2-3 tuần
	- Khách hàng tham gia vào tiến trình phát triển: phát biểu yêu cầu, ưu tiên yêu cầu, phản hồi.
4. Tuyên ngôn của Agile (triết lý)
	- vai trò, nỗ lực năng lực từng thành viên
	- Sự tương tác giữa các thành viên trong nhóm và với khách hàng
		=> Đề cao hơn quy trình và công cụ
	- Sự đáp ứng nhu cầu, chất lượng của bản thân Phần mềm 
		=> Tài liệu
	- Phản hồi, chấp nhận thay đổi, với mỗi thay đổi có 1 kế hoạch nhỏ trong thời gian ngắn. 
		=> Theo kế hoạch
1. 1 số note:
	- Hạn chế tài liệu, thay vào đó là trao đổi thường xuyên giữa con người
	- Đề cao viết mã có cấu trúc tốt và dễ đọc, đầu tư công sức vào cải tiến mã

## Thu thập và phân tích yêu cầu 

### I. Một số khái niệm cơ bản

1. Yêu cầu: 
	Các mô tả (từ mức chung đến chi tiết) về các dịch vụ hệ thống cùng với các ràng buộc
2. Mục đích chính của yêu cầu
	- Cơ sở cho đề xuất/ đấu thầu, hợp đồng
	- Cơ sở cho lập hợp đồng 
3. Phân loại yêu cầu ( làm top down từ mức cao -> thấp dần
	- Theo mức trừu tượng:
		- Yêu cầu người dùng: Ứng với từng tính năng của người sử dụng; ngôn ngữ tự nhiên + biểu đồ -> mô tả các dịch vụ mà hệ thống cung cấp; viết cho người dùng (từ chung -> chi tiết)
		- Yêu cầu hệ thống: Đặc tả chi tiết -> nên ra các dịch vụ của hệ thống và chi tiết của nó; Xác định những gì cần được phát triển, cài đặt -> đôi khi còn là đặc tả chức năng (1 phần nội dung hợp đồng)
	- Theo yêu cầu:
		- Yêu cầu chức năng: mô tả chức năng, dịch vụ của hệ thống, cách hệ thống phản ứng với môi trường và các hoạt động quan sát được của hệ thống
			-> Phụ thuộc vào loại phần mềm cần xây dựng, sự mong đợi của người dùng, quy mô hệ thống được phát triển và môi trường đích
		- Yêu cầu phi chức năng: ràng buộc mà hệ thống phải đáp ứng
			- Quy trình phát triển, công nghệ phát triển
			- Yêu cầu về sản phẩm, an ninh chịu tải
		- Yêu cầu miền: Phụ thuộc và miền nghiệp vụ, lĩnh vực. Đặc thù các lĩnh vực cụ thể, nghiệp vụ riêng …
			- Miền hoạt động của hệ thống thường đặt ra thêm các yêu cầu mới. 
			- Khi các yêu cầu miền không ổn thỏa, thì hệ thống có thể không hoạt động
			-> Quan trọng vì phản ánh những cơ sở nền tảng của miền ứng dụng

### II. Quy trình thu thập, phân tích và đặc tả yêu cầu

- Input của pha: Kế hoạch dự án
- Output của pha: tài liệu đặc tả yêu cầu (SRS)
Mục tiêu: Xác định tất cả các yêu cầu của sản phẩm 1 cách chi tiết, đầy đủ, chính xác nhất

1. SRS: Quan trọng bậc nhất, đính kèm hợp đồng, có giá trị pháp lý, so sánh khi nghiệm thu
	- Là phát biểu chính thống về những gì cần phải đạt được cho việc phân tích phần mềm
	- Gồm: định nghĩa về các yêu cầu người dùng -> tài liệu xây dựng yêu cầu; bản đặc tả các yêu cầu hệ thống -> tài liệu đặc tả yêu cầu
2. Tính chất của yêu cầu:
	- Tính chính xác
		- Phát sinh vấn đề khi các yêu cầu được mô tả không chính xác
		- Các yêu cầu nhập nhàng sẽ được hiểu và cài đặt theo những cách khác nhau
	- Tính đầy đủ và nhất quán
		- Tất cả các chức năng mà người dùng cần ở hệ thống phải được xác định
		- Các yêu cầu nêu ra không được mâu thuẫn với nhau
			-> Đối với hệ  thống phức tạp, điều này rất khó <không thể> đạt ngay được
	- Tính đo được:
		- Các yêu cầu phi chức năng cần phải được lượng hóa để có thể kiểm tra tính thỏa mãn của sản phẩm
		- Các yêu cầu PCN thường được gắn với các tiêu chí thỏa mãn để kiểm tra và thẩm định
3. Yêu cầu cho tài liệu PM
	- Chỉ mô tả các hoạt động của hệ thống từ bên ngoài
	- Chỉ ra được các ràng buộc của hệ thống trong quá trình vận hành
	- Dễ thay đổi
	- Phục vụ như tài liệu tham khảo cho người bảo trì hệ thống
	- Dự đoán trước được vòng đời của hệ thống
	- Mô tả được các đáp ứng đối với những sự cố, thay đổi ngoài dự tính
	Có chuẩn ISO cho SRS hoặc mỗi công ty có 1 chuẩn riêng < format, nội dung >   
	-> Vẫn luôn tập trung vào yêu cầu của khách hàng là gì?   
	Dùng ngôn ngữ thông thường -> tất cả các bên có thể hiểu biết (dùng chuyên môn thì phải có giải thích)   
4. Quy trình thu thập, phân tích và đặc tả yêu cầu gồm bốn bước:
		Thu thập yêu cầu -> Phân tích yêu cầu -> Đặc tả -> Thẩm định -> Lập lại   
		-> Lập đi lập lại càng sau càng rõ càng chính xác. Lập lại đến khi có được tài liệu các bên chấp nhận.   
	- Thu thập yêu cầu: Tìm hiểu về miền ứng dụng, các dịch vụ hệ thống cung cấp, các ràng buộc của hệ thống. Có rất nhiều kĩ thuật, phỏng vấn, bản mẫu, quan sát, nghiên cứu hệ thống hiện tại, nghiên cứu tài liệu, chuyên gia
		-> Phối hợp nhiều kỹ thuật. Thường : đầu tiên phỏng vấn -> yêu cầu sơ bộ dùng bản mẫu/ quan sát -> hiểu chi tiết thêm
		-> Output: 1 loạt các yêu cầu (có cả yêu cầu chưa rõ, mâu thuẫn …)
		- Kỹ thuật phỏng vấn
			- Nội dung: hỏi đáp 1 cách hình thức hoặc không hình thức với các bên liên quan
			Có phỏng vấn đóng và mở
			Tip Hướng người được phỏng vấn tham gia tình huống được thiết kế, sử dụng bản câu hỏi, bản đề xuất yêu cầu, bản mẫu hệ thống
			- Ưu điểm: Cung cấp cái nhìn tổng quan về các bên liên quan
			- Hạn chế: Người phân tích yêu cầu gặp khó khăn với tri thức miền, 1 vài tri thức miền không được phải biểu tường minh.
		- Kỹ thuật dùng kịch bản
			- Nội dung: Sử dụng các ví dụ và phân ví dụ trong thực tế về cách sử dụng hệ thống, Cung cấp các nội dung theo tình huống: thời điểm bắt đầu, kết thúc, dòng sự kiện …
			- Kỹ thuật cao sử dụng
				- Dựa vào kịch bản
				- Mô tả tập chức năng từ góc nhìn người dùng
				- Mô tả tương tác các actor và hệ thống
		- Kỹ thuật nghiên cứu nhân học:
			- Nội dung: dành thời gian quan sát - phân tích các hoạt động nghiệp vụ trong thực tế (người thực hiện không cần giải thích)
			Các yếu tố tổ chức và xã hội được nắm bắt
			- Đặc điểm: Các thực hiện trong thực tế có thể khác quy trình.
			Hiệu quả để hiểu hệ thống hiện tại nhưng không cho phép xác định thuộc tính mới. Thường kết hợp với bản mẫu
	- Phân tích yêu cầu (BA)
		Giải quyết những cái chưa rõ, mâu thuẫn, ..   
		Bản chất là BA giàu kinh nghiệm, hiểu -> đọc -> đánh giá, phản biện (có hợp lý không, có hiệu quả trong ứng dụng CNTT không? Có chính xác không?)   
		Đánh giá xem yêu cầu đó khách hàng có thực sự muốn không? Cái nói ra khác mong muốn khác hướng đến   
		-> Lý tưởng là tư vấn ngược lại khách hàng về quy trình nghiệp vụ   
		-> Output: Các yêu cầu đã rõ ràng, chính xác theo các tiêu chuẩn (3 tính chất)    
	- Đặc tả yêu cầu: làm tài liệu SRS, mô tả kết quả phân tích = một ngôn ngữ nào đó, thông thường là ngôn ngữ tự nhiên + UML. Chất lượng cực cao, ngôn ngữ hình thức, biểu đồ, bảng điểm
	- Ngôn ngữ tự nhiên
		- Các yêu cầu được diễn đạt bằng ngôn ngữ tự nhiên và được gắn với các chỉ số
		- Ưu điểm: dễ dàng, tự nhiên và phổ biến
		- Hạn chế: Nhập nhằng, hỗn tạp dễ hiểu nhầm vì ngữ cảnh khác nhau. Khó tách biệt yêu cầu của chức năng và phi chức năng; Khó đảm bảo đồng thời tính chính xác và dễ đọc
	- Các ký pháp đồ họa:
		 Sử dụng các biểu đồ đồ họa để bổ trợ cho các diễn đạt ngôn ngữ, trung hòa 2 cái còn lại   
	- Đặc tả hình thức:
		 Sử dụng ngôn ngữ, mô hình toán học để đặc tả hệ thống   
		- Ưu điểm: Tính chính xác rõ ràng, không nhập nhằng
		- Nhược điểm: Khó khăn trong chuyển từ ngôn ngữ tự nhiên sang công cụ đặc tả toán (Khó hiểu và cần chuyên gia)
		 -> Áp dụng cho những app đặc biệt không được phép sai trong quân sự, an ninh
	- Thẩm định yêu cầu: 
		- Đảm bảo các yêu cầu sẽ xác định đúng hệ thống mà khách hàng mong đợi
		- Tự thẩm định, đưa cho khách hàng thẩm định: kiểm tra đánh giá, phân tích thủ công, làm bản mẫu, sinh ca kiểm thử

## Mô hình hệ thống hóa

### I. Khái niệm cơ bản
- Hệ thống bao gồm các thành phần (thiết bị, phần mềm, con người) hoạt động trong môi trường và hướng mục đích
- Mô hình hóa hệ thống, sự đơn giản hóa của chủ thể trong thế giới thực
- Mục đích của mô hình hóa hệ thống:
	- Để hiểu tổng thể hệ thống (chức năng, cấu trúc) và để giao tiếp với các bên liên quan
	- Mô hình hệ thống hiệu thời -> giúp cho thu thập và phân tích yêu cầu
	- Mô hình hệ thống mới (phân tích, thiết kế, cài đặt): Đặc tả yêu cầu hệ thống, Đề xuất thiết kế hệ thống, Làm tài liệu
	- Nguyên lý mô hình hóa hệ thống
	- Các góc nhìn hệ thống (từ bên ngoài, tương tác, cấu trúc, hành vi)

### II. Xây dựng biểu đồ UC

1. Mô hình sử dụng
	- Đặc tả và cấu trúc yêu cầu hệ thống
	- Mỗi case sử dụng đại diện cho 1 tác vụ rời rạc có liên quan đến sự tương tác bên ngoài với hệ thống (chức năng cung cấp cho 1 loại actor cụ thể)
	- Thường ở dạng kết hợp biểu đồ trực quan và các mô tả văn bản chi tiết 
2. Biểu đồ UC
	- Actor: 1 lớp người, tổ chức, thiết bị hoặc thành phần phần mềm, bên ngoài tương tác với hệ thống
	- UC: Đại diện cho các hoạt động được thực hiện bởi một hoặc nhiều tác nhân trong việc theo đuổi một mục tiêu cụ thể
	- Các quan hệ:
		- Tổng quát hóa (giữa các actor) và giữa các UC: kế thừa, cha có gì con có nấy -> thể hiện rõ hơn các yêu cầu
		- Include: Quan hệ bắt buộc phải có để base UC xảy ra thì bắt buộc included UC xảy ra. Bóc tách ra (dựa vào độ lớn UC và khả năng tái sử dụng) do Included UC dùng nhiều lần (cung cấp dịch vụ hoàn chỉnh lập đi lập lại trong những UC khác nhau). Included UC không đứng một mình, không là UC trực tiếp của 1 actor nào cả
		- Extend: Quan hệ mở rộng (không bắt buộc - có thể có hoặc không). Trong quá trình thực hiện UC này có thể thực hiện UC khác (optional). Extended UC có thể đứng một mình 
3. Xây dựng UC Diagram
	- Sử dụng phương pháp phân tích hướng đối tượng + sự tương tác giữa các đối tượng với nhau
	- Các bước:
		- Xác định danh sách actors
		- Xác định UCs cho từng actor
		- Làm mịn: chia 1 UC -> nhiều UC nhỏ. Mịn nữa -> thành một dịch vụ hoàn chỉnh, độc lập
		- Xác định mối quan hệ actor - actor; UC - UC
		- Vẽ
### III. Xây dựng biểu đồ lớp

1. Biểu đồ lớp
	- Biểu diễn mô hình cấu trúc hệ thống (hệ thống xử lý những dữ liệu gì)
	- Lớp: tập các đối tượng cùng đặc điểm, hành vi, ngữ nghĩa
	- Các quan hệ:
		- Kết hợp: quan hệ ngữ nghĩa giữa các lớp
		- Tổng quát hóa: lớp con chi tiết hóa lớp cha
		- Tụ hợp (hợp thành): tổng thể và bộ phận, có (ko có) thành phần chia sẻ
2. Các bước xây dựng
	- Xây dựng biểu đồ lớp cho từng UC
	- Merge lại, chú ý tên các class thống nhất
3. Cách mô tả hệ thống
	- Mô hình ngữ cảnh (môi trường của hệ thống)
	- Mô hình cấu trúc (tổ chức và kiến trúc hệ thống): class
	- Mô hình behavior (UC, trần tự)

## Thiết kế kiến trúc

### I.  Định nghĩa kiến trúc PM và một số khái niệm

1. Kiến trúc PM: là bản thiết kế cho việc xây dựng và tiến hóa phần mềm
	Kiến trúc PM: là tập hợp các cấu trúc cần thiết để lập luận về hệ thống bao gồm các phần tử phần mềm, các mối quan hệ giữa chúng và thuộc tính của cả 2   
	Cấu trúc = tập các phần tử: component, sub system, module, … cụm các dịch vụ liên quan đến nhau phục vụ 1 số actors   
	Cách tổ chức: quyết định các phần tử tương tác với nhau như thế nào, cơ chế là gì
	-> Nhìn vào kiến trúc là biết được:
	- Gồm nhiều TP nào 
	- Các TP tương tác với nhau
	- Các thuộc tính cơ bản của hệ thống (module, thành phần kết nối, phân phối
2. Vai trò của kiến trúc phần mềm:
	- Công cụ giao tiếp giữa các bên liên quan
	- Để phân tích hệ thống: tiến hành những hoạt động thiết kế có tác động sâu sắc đến hệ thống sau này
	- Giúp sử dụng lại ở quy mô lớn: kiến trúc thu được có thể dùng cho các hệ thống có yêu cầu tương tự
	- Đối với người kĩ sử:
		- Tăng cường hiểu biết về hệ thống cần xây dựng: mô tả hệ thống ở nhiều khía cạnh khác nhau -> dễ hình dung hệ thống đầy đủ, chính xác
		- Phân tích hiệu quả: dự đoán chất lượng hệ thống, dự trù chi phí, thời gian xây dựng hệ thống
		- Xem xét sửa đổi kiến trúc từ sớm nếu rủi ro cao
3. Mẫu kiến trúc: kiến trúc được sử dụng để giải quyết một vài vấn đề khi xây dựng hệ thống đã được sử dụng nhiều hệ thống 
4. Các thuộc tính chất lượng: Đánh giá là một kiến trúc tốt
	- Linh hoạt (quan trọng): do một trong những yêu cầu của hệ thống là có khả năng mở rộng, thay đổi (mặt thiết với sự phụ thuộc giữa các thành phần)
	- Khả chuyển: thay đổi môi trường triển khai
	- Khả năng sử dụng lại (một phần/toàn bộ cho phần mềm khác)
	- Tips: 
		- Để hiệu năng cao : tiến trình song song, quản lý lượng và tần suất lữ liệu trao đổi giữa các tiến trình, xác định nút cổ chai về hiệu năng trong hệ thống
		- Để có an ninh tốt: cấu trúc phần mềm thành nhiều tầng, phân quyền chức năng 

### II. Tiến trình thiết kế kiến trúc

1. Nghiên lý thiết kế:
	- Phân tách các khía cạnh quan tâm:
		- Chia thành các thành phần mịn chồng chéo chức năng
		- Hạn chế tương tác, phụ thuộc giữa các thành phần khác nhau
		- Tăng kết dính trong từng thành phần
		- Đơn nhiệm: Mỗi thành phần chỉ thực hiện các chức năng gắn kết chặt chẽ
		- Hiểu biết tối thiểu: Như dùng thư viện, không cần biết chi tiết trong thành phần khác ntn
		- Không lập lại: Tồn tại 2 thành phần cung cấp 1 dịch vụ
		- Hạn chế thiết kế trước: Chỉ thiết kế khi cần và đủ thông tin
2. Quy trình thiết kế kiến trúc
- Input: Yêu cầu chức năng và phi chức năng, các ràng buộc 
- Output: Bản thiết kế kiến trúc
- Quá trình lập lại với 5 bước chính:
	- Xác định mục tiêu
	- Xác định các hoạt cảnh sử dụng chính
	- Tổng quan về ứng dụng
	- Xác định các vấn đề chính
	- Xác định giải pháp chính

### III. Một số kiểu kiến trúc phổ biến

1. Kiểu khách - chủ (kiến trúc theo cách tổ chức dữ liệu)
	- Tư tưởng lớp: 
		Toàn bộ xử lý (tính toán, …) trên host, client chỉ request và nhận kết quả, view -> hiệu xuất tối ưu do phần nặng nhất nằm trên 1 mình server, dữ liệu chia sẻ tối thiểu, băng thông tối ưu
	- Biến thể:
		- Client - Queue - Client
		- P2P
		- App server
2. Kiểu phân lớp
	- Nhóm các chức năng có liên quan chặt chẽ vào một lớp
	- Các lớp xếp chồng lên nhau
	- Chỉ lớp trên mới sử dụng chức năng lớp dưới -> mịn hơn: nhìn rõ hơn thành phần gì, tương tác như thế nào nếu chia nhiều lớp -> biểu diễn sáng sủa nhưng hiệu xuất lại chậm
3. Kiểu ống nhẫn và bộ lọc
	- Dữ liệu truyền qua các ống dẫn để đến và được xử lý ở bộ lọc
	- Trương tác giữa các component rõ: mô tả chi tiết tương tác giữa các thành phần và bên trong các thành phần
4. Kiểu bus thông điệp
	- Tương tác giữa các thành phần trong hệ thống = cách truyền thông điệp trên 1 bus chung

## Thiết kế UI UX

### I. Khái niệm
- UI bao gồm phần mềm và có thể có thiết bị (bút tương tác…)
- UX: tất cả khía cạnh tương tác của người dùng với dịch vụ và sản phẩm đáp ứng nhu cầu …

### II. Tầm quan trọng của thiết kế giao diện người dùng

- Người dùng khai thác tính năng của hệ thống thông qua UI
	-> Thường đánh giá về hệ thống thông qua đánh giá UI hơn là tính năng
- UI tồi: người dùng gây ra lỗi, dẫn đến việc phần mềm không bao giờ được sử dụng

### III. Quy trình thiết kế UI

- Input: Tài liệu yêu cầu (mô tả chi tiết UC)
	- Kịch bản các hoạt động của người dùng
	- Phản hồi của hệ thống
- Output: 
	- Kịch bản người dùng tương tác với Phần mềm thông qua giao diện
	- Bổ túc màn hình hiển thị
- Quy trình: 
	- Phân tích người dùng: Đưa data vào thế nào, hệ thống biểu thị data ra như thế nào
	- Thiết kế giao diện: Làm bản mẫu, sử dụng các phương pháp mô tả giao diện
	- Xây dựng giao diện
	- Thẩm định giao diện

 ### IV. Nguyên tắc thiết kế UI
 
- Giao diện thân thiện với người dùng, sử dụng thuật ngữ, khái niệm hướng người dùng chứ không hứa máy tính (404 ..)
- Nhất quán: Các thứ tg tự nhau nên hoạt động theo cách giống nhau (thực đơn cùng định dạng…)
- Không gây bất ngờ lớn cho người dùng
- Khả năng phục hồi cho phép quay lại trạng thái trước khi gây ra lỗi
- Có hướng dẫn người dùng
- Hướng tới đa dạng người dùng
  
## Thiết kế chi tiết

## Implementation

Quá trình chuyển từ design sang sản phẩm là Implementation   
- Input: Thiết kế chi tiết
- Output: Chương trình, sản phẩm phần mềm tốt, mã nguồn dễ bảo trì, ít hỏng
- Chiến lược Implementing (do công ty quy định)
	- Tăng cường reuse: thư viện các service của công ty; xem thị trường có bán không? Code là giải pháp cuối cùng khi không reuse được
	- Khi code tuân thủ code convention
- Kỹ thuật lập trình chuyên nghiệp:
	- Tuân theo các chuẩn viết mã nguồn
	- Các chuẩn quy định do Ngôn ngữ lập trình, do Công ty
- Kỹ thuật lập trình hiệu quả:
	- Dễ bảo trì: dễ hiệu, dễ fix
	- Khả năng tái sử dụng cao -> chú thích rõ, đủ
	- Sử dụng các cấu trúc an toàn: Mẫu thiết kế; lỗi, Bắt lỗi, ngoại lệ 
- Phong cách lập trình: 
	- Đặt tên biến, tên hàm
	- Câu lệnh: Mô tả cấu trúc (thụt lề…); Làm đơn giản các câu lệnh (mỗi câu 1 dòng …); trách cấu trúc phức tạp (lệnh lồng nhau …)

## Kiểm thử

### I. Verification and Validation
1. Verification
	- Input: Correct design (SO vs SRS) D đã Implement thành II 
	- Output: trả lời câu hỏi: sản phẩm có được cài đặt đúng thiết kế không?
		-> phát hiện lỗi lập trình so với thiết kế
2. Validation
	- Input: SRS đã được design D và cài thành II
	- Output: trả lời câu hỏi sản phẩm có đáp ứng yêu cầu khách hàng không (chức năng, phi chức năng) -> tìm lỗi phân tích thiết kế 
3. V&V: Verification -> Validation (đúng thứ tự)
	- Thể hiện người tắc làm việc: mình làm đúng không phải kiểm tra trước khi bàn giao với lead
	- Valid trước thì lỗi sẽ không biết do đâu
4. Có 2 cách làm V&V
	- Tĩnh:
		- Không execute II
		- Xét duyệt yêu cầu, thiết kế, mã: phân tích mã nguồn, code review
		- Tiến hành với mọi giai đoạn phát triển phần mềm
		- Khó đánh giá tính hiệu quả của phần mềm nhưng tổng quát hóa hơn
	- Động
		- Execute II
		- Là cách duy nhất các yêu cầu phi chức năng

### II. Kiểm thử phần mềm
Là V&V động   
Là hoạt động chủ chốt nhằm đánh giá chất lượng   
1. Các hoạt động kiểm thử:
	- Xác định -> Thiết kế -> Xây dựng -> Chạy -> So sánh
		-> Chất lượng kiểm thử phụ thuộc và bộ test II
2. Mục tiêu: 
	- Chứng minh với khách hàng là phần mềm đáp ứng các yêu cầu của nó
	- Tìm lỗi
3. Bộ kiểm thử tốt:
	- SRS - SUT: system  under testing: là 1 unit/cả hệ thống
		-> Tiêu chuẩn bao phủ định hướng thiết kế các test case
	- Các chiến lược sinh bộ kiểm thử:
		- Kiểm thử hộp đen: sinh test từ đặc tả, không cần biết code. Kiểm thử hàm/kiểm thử chức năng -> thích hợp tất cả cấp độ kiểm thử
		- Kiểm thử hộp trắng: sinh test từ SUT. Kiểm thử cấu trúc/kiểm thử logic. Tiêu chuẩn bao phủ: dòng lệnh, nhánh, đường đi, vòng lặp
			-> Kiểm tra những gì đã làm, kiểm tra những gì cần được làm. Không thích hợp cho kiểm thử hệ thống và tích hợp
	- Kiểm thử và debugging
		- Kiểm định có lỗi
		- Định vị lỗi và sửa lỗi -> lập giả thuyết về hành vi chương trình và kiểm tra các giả thuyết này
	- Các mức kiểm thử: 
		- Đơn vị -> Tích hợp -> Hệ thống -> Chấp thuận
		- Mã đơn vị -> Kiểm thử đơn vị -> Kiểm thử hệ thống -> Kiểm thử chất lượng -> Kiểm thử chấp thuận -> Kiểm thử cài đặt, môi trường …
	- Khi nào dừng kiểm thử:
		- Hết thời gian, ngân sách
		- Đạt mức độ, bao phủ mong muốn
		- Đạt tần suất hỏng hóc mong muốn
	- Kiểm thử hồi quy
		- Khi một hệ thống được chỉnh sửa, toàn bộ kiểm thử phải được chạy lại.
			-> Đảm bảo các tính năng đang hoạt động tốt không bị ảnh hưởng

### III. Một số phương pháp kiểm thử

1. Phân tích giá trị biên
	- Các chương trình bằng một hàm
	- Mục tiêu: sử dụng kiến thức về hàm để xác định các ca kiểm thử: sử dụng miền giá trị hoặc miền xác định
		-> Tập trung vào biên của miền xác định
		-> Hiệu quả với các chương trình có đầu vào độc lập/biểu diễn đại lượng vật lý bị chặn
	Lấy ca kiểm thử mà không tính đến chức năng hàm hay ý nghĩa biến 
2. Phân hạch tương đương
	- Cảm giác kiểm thử hết (hợp các lớp = miền đầu vào). Tránh dư thừa (2 lớp bất lù không giao nhau)
	- Ý tưởng: chỉ kiểm thử 1 phần tử ở mỗi miền tương tương
		-> Giảm nhiêu dư thừa nếu chọn các lớp tương đương hợp lý
		-> Mấu chốt: chọn được quan hệ tương đương
	- Chọn phân hoạch: cần hiểu về miền xác định, hiểu đầu vào phụ thuộc nhau như thế nào

## Quản lý dự án

### I. Dự án
1. Khái niệm “Dự án"
	- Tập các công việc
	- Được thực hiện bởi nhóm người có chuyên môn
	- Tạo ra một sản phẩm/dịch vụ duy nhất
	- Sử dụng nguồn lực dự biến (thời gian, kinh phí, người)
2. Dự án CNTT - dự án PM:
	- Sản phẩm: một hệ thống thông tin
	Triển khai khi: môi trường ( chưa có phần cứng, data)
	- Sản phẩm: một phần mềm/ dịch vụ phần mềm
	Triển khai khi: có sẵn mọi thứ
3. Các tiêu 1 dự án thành công
	- Thỏa mãn bộ 3: scope goal, cost goal, time goal
	- Thỏa mãn khách hàng, chủ đầu tư
	- Thỏa mãn các bên liên quan

### II. Quản lý dự án

Là lập kế hoạch và thực hiện các công việc theo đúng kế hoạch đã lập
1. Các bước:
	- Định nghĩa dự án
	- Lập khách hàng
	- Triển khai, tổ chức thực hiện
	- Kiểm tra giám sát
	- Kết thúc dự án
2. Mục đích quản lý dự án:
	- Là giảm tỷ lệ thất bại, giúp dự án đạt mục tiêu đề ra
3. 10 miền tri thức trong Quản lý dự án:
	- Scope: Phạm vi dự án
	- Time
	- Cost: Dự toán chi phí, gồm những gì, bao nhiêu
	- Quality: chất lượng
	- Communication: Các thành viên, các biên liên quan, nhà thầu
	- HR: nhân lực, phân công, động viên, nhắc nhở
	- Risk: Rủi ro
	- Processment: Quy trình, thủ tục
	- Stakeholder: Ông nào quan trọng, sở thích sở ghét
4. Trong các bên liên quan: 
	Quan trọng nhất: nhà tài trợ - chủ đầu tư, khách hàng, tổ dự án, quản lý cấp cao, bên thứ 3 
	-> Kết nối quan trọng nhất là quản lý dự án