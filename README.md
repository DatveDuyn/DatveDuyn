import time
import os

def clear_screen():
    # Xóa nội dung trên màn hình bằng cách gửi lệnh đến hệ điều hành tương ứng
    os.system('cls' if os.name == 'nt' else 'clear')

def send_message():
    messages = [
        "Chào Duy",
        "Tớ là Liên",
        "Tớ có điều này muốn nói với cậu lần nữa :33",
        "Tuy nhiên",
        "Việc cậu cảm thấy như thế nào thì cậu hãy suy nghĩ thật kĩ nhé (●'◡'●)",
        "Bởi vì",
        "Có lẽ đây sẽ là lần cuối cùng tớ nói với cậu điều này",
        "Cậu là người mà tớ thích thầm lâu nhất",
        "Là người thường mang vui đến cho tớ",
        "Là người mà tớ chỉ cần nghe cậu nói chuện cũng cảm thấy vui",
        "Là người thường tạo ra cho tớ nhiều ý tưởng",
        "Là người mà tớ trân trọng nhất trong tất cả bạn bè"
    ]

    for message in messages:
        print(message)
        time.sleep(2)  # Thời gian đủ để đọc mỗi dòng
        clear_screen()  # Xóa nội dung trước khi hiển thị dòng tiếp theo

# Gọi hàm để hiển thị tin nhắn một cách chuyển động với hiệu ứng biến mất
send_message()
