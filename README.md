# MamFlow Design System & AI Skills

Hệ thống quy chuẩn thiết kế sản phẩm và chỉ dẫn lập trình dành riêng cho hệ sinh thái **MamFlow**. Bộ tài liệu này được cấu trúc dưới dạng các **AI Skills** (tệp Markdown chỉ dẫn) để giúp các mô hình AI (như Claude, GPT, Cursor, Gemini) và lập trình viên cộng tác thiết kế, phát triển sản phẩm một cách đồng bộ, nhất quán và hiệu quả.

---

## 🚀 Công Dụng Chính

1. **Chuẩn hóa Giao diện (UI/UX):** Định nghĩa chặt chẽ hệ màu sắc, kích thước khoảng cách (spacing), kiểu chữ (typography), và cấu trúc layout dành riêng cho các công cụ chuyên nghiệp và giao diện quản trị WordPress (`wp-admin`).
2. **Định tuyến Tác vụ Tự động (Task Routing):** Giúp AI tự động nạp các tệp hướng dẫn phù hợp dựa trên ngữ cảnh công việc của người dùng (từ lên kế hoạch tính năng, viết tài liệu, cho đến sinh mã HTML/Tailwind).
3. **Giảm Thiểu Lỗi Thiết Kế:** Thiết lập các "Design Guardrails" (Rào cản thiết kế) nhằm loại bỏ các xu hướng thiết kế quá đà, không thực tế, tập trung tối đa vào hiệu suất và trải nghiệm của người dùng chuyên nghiệp.

---

## 📂 Cấu Trúc Thư Mục & Ý Nghĩa Từng Tệp

Toàn bộ các quy tắc nằm trong thư mục `/backend` bao gồm:

*   **[`backend/backend-design-rules.md`](file:///d:/devland/mamflow/mamflow-design-system-skill/backend/backend-design-rules.md):** 
    *   *Vai trò:* **Điểm truy cập chính (Entry Point)** của toàn bộ hệ thống.
    *   *Nội dung:* Bản đồ định tuyến tác vụ (Task Routing), thứ tự ưu tiên khi xảy ra xung đột (Conflict Resolution), các rào cản thiết kế chung và bộ câu hỏi kiểm định cuối cùng (Final Validation) trước khi xuất kết quả.
*   **[`backend/mamflow-product-principles.md`](file:///d:/devland/mamflow/mamflow-design-system-skill/backend/mamflow-product-principles.md):**
    *   *Vai trò:* **Triết lý sản phẩm**.
    *   *Nội dung:* Xác định đối tượng người dùng (Agencies, Freelancers, Developers...) và 5 nguyên tắc cốt lõi: *Tôn trọng thời gian (Respect Time), Rõ ràng hơn Sáng tạo (Clarity Over Creativity), Công năng đi trước Trang trí (Function Before Decoration), Nhất quán là trên hết (Consistency Wins), và Giảm tải nhận thức (Reduce Cognitive Load).*
*   **[`backend/mamflow-visual-language.md`](file:///d:/devland/mamflow/mamflow-design-system-skill/backend/mamflow-visual-language.md):**
    *   *Vai trò:* **Hệ thống ngôn ngữ trực quan**.
    *   *Nội dung:* Quy định mã màu Primary (`#2563EB`), bảng màu trung tính, độ tương phản tiêu chuẩn (WCAG AA), cách dùng Icon, và các biến thể Button được phép (chỉ có 3 loại: Primary, Secondary, Danger).
*   **[`backend/mamflow-design-system.md`](file:///d:/devland/mamflow/mamflow-design-system-skill/backend/mamflow-design-system.md):**
    *   *Vai trò:* **Hệ thống thiết kế chi tiết (Design Tokens & Elements)**.
    *   *Nội dung:* Spacing Scale nghiêm ngặt (4px, 8px, 12px, 16px, 24px, 32px, 48px), cỡ chữ, cấu trúc layout chuẩn (Header -> Context -> Filters -> Content -> Actions -> Pagination), tiêu chuẩn thiết kế Bảng dữ liệu (Tables), các trạng thái Empty/Loading (Skeletons) và cách viết thông báo lỗi mang tính xây dựng.
*   **[`backend/mamflow-feature-design-skill.md`](file:///d:/devland/mamflow/mamflow-design-system-skill/backend/mamflow-feature-design-skill.md):**
    *   *Vai trò:* **Hướng dẫn thiết kế tính năng**.
    *   *Nội dung:* Quy chuẩn lập tài liệu mô tả tính năng mới (PRD/Spec) bao gồm: Mục tiêu, Đối tượng, Luồng xử lý chính (dưới 5 bước), Phân cấp thông tin, Quyền hạn (Permissions) và các kịch bản Edge Case.

---

## 🛠️ Hướng Dẫn Sử Dụng Với AI (Prompting Guide)

Khi bạn làm việc với một AI Coding Assistant (như Cursor, GitHub Copilot, hoặc ChatGPT/Claude), hãy đính kèm hoặc yêu cầu AI đọc tệp `backend/backend-design-rules.md`. 

### Cách cấu hình trong System Prompt / Cursor Rules:
Bạn có thể thêm chỉ thị sau vào `.cursorrules` hoặc System Prompt của bạn:
> "Khi xử lý bất kỳ tác vụ nào liên quan đến giao diện, tính năng hoặc nội dung của MamFlow, bạn phải luôn đọc và tuân thủ nghiêm ngặt các quy định trong tệp `backend/backend-design-rules.md` và các tệp liên quan được định tuyến trong đó."

### Phân loại định tuyến tác vụ (Task Routing):
AI sẽ tự động nạp thêm các tài liệu bổ sung dựa trên tác vụ bạn yêu cầu:
*   **UI/UX Design:** Nạp thêm `product-principles`, `visual-language`, `design-system`, `feature-design-skill`.
*   **Feature Planning (Lập kế hoạch):** Nạp thêm `product-principles`, `feature-design-skill`.
*   **UI Review (Đánh giá giao diện):** Nạp thêm `product-principles`, `visual-language`, `design-system`.
*   **HTML/Tailwind CSS Generation:** Nạp thêm `product-principles`, `visual-language`, `design-system`.
*   **WordPress Plugin UI:** Tuân thủ các nguyên tắc bản địa hóa giao diện trong `wp-admin`.

---

## ⚠️ Nguyên Tắc Thiết Kế Tối Kỵ (Design Guardrails)

Để giữ cho sản phẩm MamFlow luôn mang tính **Tin cậy - Hiệu quả - Kỹ thuật - Tập trung**, tuyệt đối **KHÔNG** được thực hiện các điều sau:
*   ❌ Không sử dụng Gradients màu.
*   ❌ Không sử dụng hiệu ứng Glassmorphism (kính mờ).
*   ❌ Không sử dụng đổ bóng quá đà (Excessive shadows).
*   ❌ Không thiết kế bảng điều khiển nhiều màu sắc sặc sỡ (Rainbow dashboards).
*   ❌ Không thêm các yếu tố trang trí vô nghĩa.
*   ❌ Không tự ý đưa vào các mã màu mới ngoài danh sách đã quy định.

---

## ⚖️ Giải Quyết Xung Đột (Conflict Resolution)

Nếu có sự mâu thuẫn về mặt hướng dẫn giữa các tài liệu, thứ tự ưu tiên áp dụng như sau (độ ưu tiên giảm dần):
1.  `mamflow-product-principles.md` (Cao nhất)
2.  `mamflow-visual-language.md`
3.  `mamflow-design-system.md`
4.  Tài liệu cụ thể của tác vụ đó.

---

## ✅ Quy Trình Kiểm Định Cuối Cùng (Final Validation)

Trước khi xuất bản giao diện hoặc tính năng, hãy tự trả lời 5 câu hỏi sau:
1.  Thiết kế này có tuân thủ các nguyên tắc sản phẩm của MamFlow không?
2.  Thiết kế này có đúng ngôn ngữ trực quan (Visual Language) không?
3.  Có tái sử dụng các mẫu thiết kế (Patterns) sẵn có không?
4.  Tính năng này có thực sự hữu ích cho người dùng chuyên nghiệp không?
5.  Có chi tiết nào bị phức tạp hóa quá mức không?

---
*Tài liệu được cập nhật tự động và đồng bộ trực tiếp với hệ thống thiết kế MamFlow.*
