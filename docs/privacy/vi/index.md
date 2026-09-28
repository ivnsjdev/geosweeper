# Chính sách quyền riêng tư cho GeoSweeper

**Ngày có hiệu lực:** 26 tháng 9 năm 2026

**Cập nhật lần cuối:** Ngày 26 tháng 9 năm 2026

## Bản rút gọn

GeoSweeper không thu thập, truyền, bán hoặc chia sẻ bất kỳ thông tin cá nhân nào. Mọi bàn cờ bạn chơi, mọi cài đặt bạn chọn và mọi quốc gia bạn đã xóa chỉ được lưu trữ trên thiết bị của bạn. Không có gì được tải lên cho chúng tôi và không có tài khoản nào để tạo ngay từ đầu. Lưu lượng truy cập mạng duy nhất mà GeoSweeper từng tạo ra là StoreKit nói chuyện với Apple khi bạn thực hiện hoặc khôi phục giao dịch mua hàng và các trang bạn cố tình mở từ một liên kết bên trong ứng dụng (trang web này hoặc các trang hợp pháp của chính Apple) — cả hai đều được đề cập bên dưới và không mang bất kỳ nội dung nào khác đi kèm.

## Chúng tôi là ai

GeoSweeper được phát triển bởi Ivan Cayabyab. Các câu hỏi về chính sách này hoặc ứng dụng có thể được gửi tới ivnsjdev@gmail.com.

## Ứng dụng lưu trữ những gì và ở đâu

Mọi thứ bên dưới chỉ tồn tại trên thiết bị của bạn, ở một trong ba nơi: `UserDefaults` (giá trị cài đặt nhỏ), tệp JSON trong thư mục Hỗ trợ ứng dụng của chính ứng dụng hoặc cơ sở dữ liệu SQLite cục bộ.

| Cái gì | Lưu trữ chính | Tự động gửi cho chúng tôi? |
|---|---|---|
| Cài đặt hiển thị - chủ đề bảng, màu neon, hiệu ứng nổ, âm thanh vụ nổ, chiếu bản đồ (quả địa cầu hoặc phẳng), bật/tắt âm thanh và xúc giác | `Mặc định của người dùng` | Không |
| Language bạn đã chọn trong ứng dụng | `Mặc định của người dùng` | Không |
| Sổ sách kế toán nhắc xếp hạng - ngày GeoSweeper yêu cầu iOS hiển thị bảng xếp hạng gốc và cột mốc nào đã kích hoạt bảng xếp hạng cuối cùng | `Mặc định của người dùng` | Không |
| Kỷ lục theo quốc gia — thắng, thua, thời điểm tốt nhất và thời điểm bạn mở khóa thành tích đó, đối với mọi quốc gia bạn đã chơi | Tệp JSON (`progress.json`) trong thư mục Hỗ trợ ứng dụng của ứng dụng | Không |
| Tiến trình Infinite Tower — hàng bạn đã tới, khung nhìn đã lưu của bạn và những hàng bạn đã xóa | Cơ sở dữ liệu SQLite cục bộ | Không |

Không có điều nào trong số này được truyền đi, bán hoặc chia sẻ với bất kỳ ai, kể cả chúng tôi. Lưu lượng truy cập của chính StoreKit (bên dưới) và các liên kết bên ngoài bạn nhấn (cũng bên dưới) không chứa lưu lượng truy cập nào. Bản sao lưu thiết bị iOS có thể bao gồm các tệp này như một phần của việc sao lưu toàn bộ ứng dụng — bản sao lưu đó do bạn hoặc iOS khởi tạo, không bao giờ bởi GeoSweeper và nó vẫn ở bất cứ nơi nào bạn gửi (iCloud hoặc máy tính của bạn), không phải với chúng tôi.

## Không có tài khoản, không đăng nhập, không có đám mây

GeoSweeper không bao giờ yêu cầu tên, địa chỉ email, số điện thoại, ngày sinh hoặc bất kỳ thông tin nhận dạng nào khác — không có gì để đăng nhập vì không có tài khoản. Tiến trình của bạn không đồng bộ hóa thông qua iCloud, CloudKit hoặc bất kỳ dịch vụ nào khác: nó chỉ tồn tại trên thiết bị bạn đang chơi. Chơi cùng một quốc gia trên thiết bị thứ hai và nó bắt đầu mới ở đó vì không có bản sao máy chủ nào để đồng bộ hóa từ đó.

## Bất cứ điều gì cố tình không tồn tại

Bàn cờ bạn đang ở giữa — mọi ô bạn đã mở, mọi lá cờ bạn đặt — chỉ được lưu giữ trong bộ nhớ khi bạn chơi. Đóng ứng dụng giữa trò chơi và bảng đó sẽ biến mất; nó không bao giờ được ghi vào đĩa và không có tính năng tự động lưu để tiếp tục một bảng chưa hoàn thành. Chỉ một trận đấu *kết thúc* (thắng hoặc thua) mới cập nhật thành tích của mỗi quốc gia được mô tả ở trên.

## Có một thứ nghe có vẻ không phải ở địa phương

Bản đồ sẽ mở ra trên quốc gia của bạn vào lần đầu tiên bạn khởi chạy ứng dụng. Điều này xuất phát từ **cài đặt vùng** của thiết bị của bạn (quốc gia gắn liền với ngôn ngữ và miền địa phương của bạn, cùng quốc gia mà iOS sử dụng để chọn bàn phím và lịch) — không phải từ GPS, Wi-Fi hoặc bất kỳ hình thức theo dõi vị trí nào khác. GeoSweeper không yêu cầu quyền truy cập vị trí và không thể đọc tọa độ của bạn ngay cả khi nó muốn.

## Quyền

GeoSweeper không yêu cầu bất kỳ quyền hệ thống nào. Nó không bao giờ yêu cầu máy ảnh, thư viện ảnh, micrô, vị trí, danh bạ, lịch, dữ liệu sức khỏe, dữ liệu chuyển động hoặc thông báo đẩy và sẽ không có bất kỳ loại lời nhắc cấp phép nào xuất hiện. Điều này khớp chính xác với `Info.plist` của ứng dụng: không có một mục mô tả sử dụng nào trong đó.

## Mua hàng

GeoSweeper được tải xuống miễn phí. 10 quốc gia đầu tiên của bạn — bất kỳ cấp độ nào, bao gồm Beginner — đều được chơi miễn phí và khi bạn đã chơi ở một quốc gia, quốc gia đó vẫn có thể chơi lại vĩnh viễn, ngay cả sau khi hết thời gian dùng thử miễn phí. Infinite Tower miễn phí tới hàng 10. Ngoài hai điểm đó, còn có hai giao dịch mua độc lập, cả hai đều là một lần, không tiêu hao và được cung cấp thông qua StoreKit của Apple và được Apple xử lý hoàn toàn:

- **All Countries** — giao dịch mua một lần, không tiêu hao để mở khóa vĩnh viễn
  Các cấp Intermediate, Expert và Mega trên tất cả 204 quốc gia. Không có gì về điều này đổi mới.
- **Infinite Tower Lifetime** — giao dịch mua một lần, không tiêu hao và mở khóa vĩnh viễn
  leo qua hàng 10. Không có gì về điều này được gia hạn và GeoSweeper không cung cấp bất kỳ hình thức đăng ký nào.

Apple, không phải GeoSweeper, xử lý mọi khoản thanh toán. Chúng tôi không bao giờ thấy số thẻ, địa chỉ thanh toán hoặc thông tin xác thực Apple Account - StoreKit chỉ cho ứng dụng biết những gì ứng dụng cần để hiển thị tường phí và cấp quyền truy cập: giá hiển thị và liệu bạn có sở hữu từng mặt hàng hay không. Những câu trả lời đó vẫn còn trên thiết bị của bạn; GeoSweeper không chạy máy chủ mua hàng riêng và không có nơi nào để gửi chúng. Khôi phục giao dịch mua yêu cầu Apple xác nhận lại những gì Apple Account của bạn sở hữu và áp dụng câu trả lời cục bộ - nó không tạo hoặc truyền bất kỳ bản ghi mới nào.

Xem thêm [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) và [EULA tiêu chuẩn](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) của Apple, quy định việc mua hàng.

## Hỗ trợ liên lạc

Nếu bạn gửi email cho ivnsjdev@gmail.com, chúng tôi sẽ nhận được địa chỉ email của bạn, bất cứ điều gì bạn viết và bất kỳ tệp đính kèm nào bạn chọn thêm vào. Chúng tôi chỉ sử dụng thông tin này để trả lời bạn và khắc phục vấn đề bạn đã viết — cơ sở hợp pháp của chúng tôi là lợi ích chính đáng của chúng tôi trong việc phản hồi những người liên hệ với chúng tôi. Hộp thư đó là tài khoản Gmail tiêu chuẩn, được Google LLC xử lý theo [Chính sách quyền riêng tư của Google](https://policies.google.com/privacy) và được lưu trữ trên cơ sở hạ tầng có thể nằm bên ngoài quốc gia của bạn. Đó là lý do tại sao việc chuyển giao đó được tiết lộ ở đây. Chúng tôi lưu giữ các email hỗ trợ trong tối đa 24 tháng và sau đó xóa chúng; bạn có thể yêu cầu chúng tôi xóa một email cụ thể sớm hơn bất kỳ lúc nào bằng cách gửi thư đến cùng một địa chỉ.

## Liên kết ngoài

Tường thanh toán của GeoSweeper liên kết với chính sách quyền riêng tư của trang web này và EULA tiêu chuẩn của Apple; Settings có thể liên kết đến trang viết đánh giá của App Store. Không có dữ liệu người dùng hoặc mã nhận dạng dành riêng cho ứng dụng nào được thêm vào bất kỳ liên kết nào trong số này — chúng là các URL đơn giản, giống nhau đối với mọi người.

## Không có gì để đánh cược

GeoSweeper không có tiền tệ trong ứng dụng, không có chiến lợi phẩm, không có rút thăm trúng thưởng và không có tính năng đặt cược hoặc đặt cược kết quả. Mỗi giao dịch mua đều là một mức giá cố định, được tiết lộ để có quyền truy cập vĩnh viễn hoặc có giới hạn thời gian vào nội dung; không có gì có thể thắng, thua hay đánh bạc.

## Những việc chúng tôi KHÔNG làm

- Không có phân tích, báo cáo sự cố hoặc đo từ xa dưới bất kỳ hình thức nào
- Không có quảng cáo, không có mạng quảng cáo và không có số nhận dạng quảng cáo
- Không theo dõi nhiều ứng dụng hoặc nhiều trang web và không có nhà môi giới dữ liệu
- Không có tài khoản, không đăng nhập, không có mật khẩu
- Không có máy ảnh, thư viện ảnh, micrô, danh bạ, vị trí chính xác hoặc thô hoặc dữ liệu sức khỏe
- Không đào tạo các mô hình học máy trên dữ liệu của bạn
- Không có SDK của bên thứ ba dưới bất kỳ hình thức nào - mã duy nhất trong ứng dụng này là của riêng chúng tôi

Điều này khớp với nhãn "Data Not Collected (dữ liệu không được thu thập)" GeoSweeper mang trên App Store.

## Giữ lại và xóa

Việc xóa ứng dụng sẽ xóa mọi tệp được lưu trữ trên thiết bị của bạn — cài đặt, hồ sơ theo quốc gia và tiến trình Infinite Tower của bạn — ngay lập tức và hoàn toàn, vì phía chúng tôi chưa bao giờ có bản sao máy chủ để chúng tôi giữ hoặc xóa. Bản sao lưu thiết bị iCloud được tạo trước khi xóa vẫn có thể chứa một bản sao; bản sao lưu đó hoàn toàn nằm dưới sự kiểm soát của bạn thông qua **Settings → tên của bạn → iCloud → Quản lý bộ nhớ tài khoản** trên thiết bị của bạn. Các email hỗ trợ được giữ lại và xóa riêng biệt như mô tả ở trên.

## Quyền của bạn

Vì GeoSweeper không giữ bản sao dữ liệu trong ứng dụng của bạn nên các quyền truy cập, chỉnh sửa, xuất và xóa mà GDPR, GDPR của Vương quốc Anh và CCPA/CPRA mô tả là những quyền bạn đã thực hiện trực tiếp trên thiết bị của mình — không có hồ sơ nào ở đây để chúng tôi tạo ra hoặc xóa thay mặt bạn. Nơi duy nhất chúng tôi lưu giữ nội dung nào đó là email hỗ trợ mà bạn đã gửi cho chúng tôi và bạn có thể yêu cầu xem, sửa hoặc xóa email đó bất kỳ lúc nào bằng cách viết thư tới ivnsjdev@gmail.com. Chúng tôi không bán hoặc chia sẻ thông tin cá nhân để quảng cáo hành vi theo ngữ cảnh và không bao giờ làm như vậy. Nếu bạn cho rằng chúng tôi đã xử lý sai dữ liệu của bạn, bạn có quyền khiếu nại với cơ quan bảo vệ dữ liệu tại địa phương.

## Trẻ em

GeoSweeper có xếp hạng độ tuổi phù hợp với khán giả nói chung và không hướng tới trẻ em cụ thể. Chúng tôi không cố ý thu thập thông tin cá nhân từ bất kỳ ai, kể cả trẻ em dưới 13 tuổi và không có gì trong ứng dụng có thể làm được điều đó — không trò chuyện, không chia sẻ, không tính năng xã hội, không quảng cáo và không có tài khoản để bên thứ ba tiếp cận trẻ em thông qua.

## Thay đổi chính sách này

Nếu chính sách này thay đổi, ngày ở trên cùng sẽ thay đổi theo và thay đổi quan trọng đối với những gì GeoSweeper thực hiện với dữ liệu cũng sẽ được ghi chú trong ghi chú phát hành của bản cập nhật đó.

## Liên hệ

ivnsjdev@gmail.com
