# Giao thức OAuth 2
### Vai trò
* Resource Owner (Chủ sỡ hữu tài nguyên)

Là người dùng hoặc hệ thống sở hữu tài nguyên có khả năng cấp quyền truy cập vào tài khoản của họ.

* Resource Server (Máy chủ tài nguyên)

Là nơi lưu trữ những tài nguyên mà người dùng chia sẻ. Server này chấp nhận và xác thực mã truy cập từ Client.

* Client (Máy khách)

Là ứng dụng muốn truy cập vào tài nguyên được bảo vệ. Muốn thực hiện được điều đó Client phải nhận được ủy quyền từ chủ sở hữu tài nguyên.

* Authorization Server (Máy chủ ủy quyền)

Là đối tượng quyết định việc cấp quyền truy cập dữ liệu cho Client. Authorization Server nhận yêu cầu từ Client sau đó xác minh danh tính người dùng và cấp mã access token để Client truy cập ứng dụng.

# Token

1. Access Token

Là một đoạn mã dùng để xác thực quyền truy cập, cho phép ứng dụng bên thứ 3 có thể truy cập vào những dữ liệu của người dùng trong một phạm vi nhất định mà nó cho phép.

2. Refresh Token

Refresh token sẽ được gửi đi để lấy về một access token mới khi nó hết hạn, cũng chính vì vậy nó có thời gian hiệu lực lâu hơn access token. 

# Scope

Scope là một tham số được định nghĩa trong Authorization server dùng để giới hạn quyền, phạm vi tài nguyên mà access token được phép truy cập. Client sẽ xác định sử dụng scope nào khi yêu cầu sinh ra một đoạn access token.

* Client Identifier: chuỗi ký tự để định danh ứng dụng

* Client Secret: chuỗi ký tự dùng để dịnh danh Client khi có yêu cầu truy cập.

