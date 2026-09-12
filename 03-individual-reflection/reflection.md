# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Phạm Xuân Quý
- Mã học viên: 2A202602745
- Nhóm: Nhóm CV Screening — 5 thành viên
- Candidate problem nhóm chọn: Hỗ trợ HR đọc, trích xuất và đối chiếu CV với tiêu chí công việc bằng OCR kết hợp multi-agent có kiểm soát; HR quyết định ứng viên đi tiếp.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tôi scan 10 vấn đề trong bối cảnh học tập, làm bài nhóm và di chuyển ở trường; sau đó chọn ba bài về tổng hợp kiến thức ôn thi, theo dõi bài giảng tiếng Anh và xếp hàng xe trước cổng trường. | Nhóm có thêm ba candidate thuộc các hướng tổng hợp tài liệu, hỗ trợ ngôn ngữ và cải tiến quy trình; Card ôn thi có baseline hơn 20 giờ/môn. |
| Pitch Problem Card | Tôi chuẩn bị pitch Card tổng hợp kiến thức khi ôn thi, nêu workflow sáu bước, bottleneck ở đọc–chọn ý chính và mục tiêu giảm từ hơn 20 giờ xuống dưới 10 giờ/môn. | Nhóm có một candidate dễ hiểu, có before/after workflow và metric để so sánh với các bài khác. |
| Challenge bài của bạn khác | Tôi tập trung hỏi liệu pain có dữ liệu thật không, giải pháp đơn giản như template/workflow đã đủ chưa và multi-agent có đang được chọn quá sớm không. | Nhóm phải ghi rõ các số liệu nào mới là giả định, bổ sung phương án đơn giản hơn và không coi tốc độ máy là toàn bộ impact. |
| Gom trùng / cluster | Tôi hỗ trợ gom 12 candidates thành bốn cụm: học tập/assignment, thông tin và tiến độ nhóm, CV/tuyển dụng, kỹ thuật/vận hành. | Nhóm nhìn thấy pattern chung “input không cấu trúc → output có cấu trúc → người kiểm tra” và rút shortlist còn ba bài. |
| Chọn candidate problem | Tôi tham gia đối chiếu ba bài shortlist theo actor, workflow, evidence, impact, khả năng làm trong lab và khả năng so sánh Rule/Workflow/Agent. | Nhóm chọn bài hỗ trợ HR sàng lọc CV, đồng thời ghi rõ đây là bước tái định nghĩa từ cụm CV/JD và cần validation riêng với HR. |
| Validation / research | Tôi tổng hợp tín hiệu nội bộ rằng hệ thống từng đạt throughput dưới 1 giây/CV và kiểm tra các nguồn về Workable, Azure Document Intelligence, Google Document AI, LangGraph và rủi ro AI tuyển dụng. | Nhóm tách được system throughput khỏi thời gian end-to-end và quyết định dùng OCR có sẵn thay vì tự xây từ đầu. |
| Workflow nhóm | Tôi rà lại current/future workflow để phân biệt bước Rule, OCR, agent và bước HR review; bổ sung nhánh confidence thấp và fallback về CV gốc. | Workflow thể hiện được machine boundary, human boundary và không cho lỗi OCR đi thẳng tới quyết định tuyển dụng. |
| Problem Statement | Với vai trò writer, tôi tổng hợp Problem Statement v0 rồi siết lại thành v1: thu hẹp vào một vị trí, 50–100 CV, rubric do HR duyệt và evidence report có nguồn. | Actor, bottleneck, metric, AI intervention point và phạm vi “làm/không làm” được diễn đạt cụ thể hơn. |
| Rule / Workflow / Agent | Tôi cùng nhóm so sánh Rule cho bước cứng, Workflow làm khung điều phối và Agent cho các nhánh OCR/extraction/matching/QA. | Nhóm chọn multi-agent có giới hạn, không chọn một agent tự do và vẫn giữ workflow cố định làm baseline để có thể hạ mức. |
| Decision | Tôi ủng hộ quyết định Not Yet vì baseline HR, bộ CV ẩn danh và benchmark tái lập chưa đủ, dù đã có tín hiệu nội bộ về tốc độ dưới 1 giây/CV. | Quyết định có pilot, metric, điều kiện Go và tiêu chí rollback thay vì kết luận quá sớm chỉ vì giải pháp nghe hấp dẫn. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là phần viết và siết Problem Statement v0 → v1, đặc biệt là tách tốc độ tầng máy khỏi thời gian HR review và đặt boundary để AI chỉ tạo evidence report, không tự động tuyển hoặc loại ứng viên.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Sau khi tự đưa ra ba vấn đề ban đầu, tôi nhờ AI gợi ý và chuẩn hóa thêm các vấn đề theo bốn lăng kính. | AI giúp mở rộng bảng thành 10 dòng và bổ sung actor, dấu hiệu đo cùng cách diễn đạt cụ thể. | Một số gợi ý và số liệu chỉ là giả định; AI còn đặt vấn đề nghe tiếng Anh vào bối cảnh khách hàng, không khớp vai trò sinh viên. | Tôi đổi actor về sinh viên–giảng viên, giữ riêng các số liệu thật đã biết và đánh dấu phần còn lại là ước lượng cần kiểm chứng. |
| Problem Card | Tôi nhờ AI cấu trúc Top 3 thành Problem Card và workflow trước/sau. | AI giúp điền đủ bottleneck, impact, success metric, non-AI alternative, hypothesis và fallback. | Phân bổ thời gian ở từng bước còn mang tính ước lượng và metric chất lượng ban đầu chưa đủ chặt. | Tôi chọn ba vấn đề gốc của mình, giữ hơn 20 giờ/môn và 15 phút chờ xe làm mốc, đồng thời thêm bước người dùng kiểm tra. |
| Workflow | Tôi dùng AI để chuyển mô tả quy trình lọc CV thành pipeline Rule → OCR → multi-agent → HR review. | AI làm rõ các agent chuyên trách, nhánh OCR confidence thấp, human boundary và rollback. | AI ban đầu trộn thời gian máy xử lý với thời gian end-to-end, khiến con số dưới 1 giây/CV dễ bị hiểu sai. | Tôi bổ sung thông tin từ thành viên từng triển khai và tách system throughput dưới 1 giây/CV khỏi tổng thời gian có HR review. |
| Research | Tôi dùng AI để tìm và tổng hợp tài liệu chính thức về OCR, document parsing, multi-agent orchestration và AI trong tuyển dụng. | AI giúp tìm nhanh Workable, Azure, Google Document AI, LangGraph và nguồn cảnh báo về rủi ro phân biệt đối xử. | Một số nguồn chỉ mô tả sản phẩm hoặc thuộc bối cảnh pháp lý Hoa Kỳ, không chứng minh pain của HR Việt Nam. | Tôi chỉ giữ link chính thức, ghi rõ khoảng trống và không dùng research thay cho interview/validation người dùng. |
| Problem Statement | Tôi nhờ AI kiểm tra các field v0 và hỗ trợ diễn đạt bản v1 chặt hơn. | AI phát hiện actor, metric, intervention point và boundary cần cụ thể hóa. | AI có xu hướng biến số liệu giả định thành baseline nghe chắc chắn và dùng cụm “CV phù hợp” quá rộng. | Tôi gắn nhãn baseline giả định, giới hạn pilot vào một vị trí, yêu cầu rubric do HR duyệt và đổi output thành evidence report có trích nguồn. |
| Rule / Workflow / Agent | Tôi dùng AI để lập bảng so sánh ba mức và phản biện việc chọn Agent. | AI chỉ ra Rule vẫn phù hợp cho file/privacy/threshold và Workflow phải là khung điều phối của hệ thống. | Nếu chỉ đi theo tên đề tài, AI dễ hợp thức hóa multi-agent mà chưa chứng minh cần autonomy. | Tôi giới hạn quyền từng agent, thêm nhánh human review và điều kiện hạ xuống workflow nếu pilot không cho lợi ích rõ. |
| Decision | Tôi dùng AI để kiểm tra mức độ sẵn sàng và viết các điều kiện Go, Not Yet, No-Go cùng rollback. | AI giúp tách rõ dữ liệu còn thiếu, pilot nhỏ nhất và các ngưỡng dừng. | AI không thể tự tạo bằng chứng validation hoặc bảo đảm claim dưới 1 giây/CV tái lập được. | Tôi giữ quyết định Not Yet, yêu cầu benchmark p50/p95 và validation với HR trước khi dùng vào ứng viên thật. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Khi nghe Top 3 của các thành viên khác, tôi nhận ra nhiều vấn đề tuy khác bối cảnh nhưng đều có pattern chung là phải biến thông tin rời rạc thành đầu ra có cấu trúc. Candidate của tôi về tổng hợp kiến thức ôn thi có impact thời gian lớn, nhưng nhóm chọn bài sàng lọc CV vì workflow nhiều bước và có thể phân tích rõ Rule, Workflow và Agent. Lúc đầu chúng tôi khá solution-first khi chú ý ngay tới multi-agent và OCR vì giải pháp nghe mạnh về công nghệ. Sau khi vẽ workflow, tôi hiểu rằng tốc độ máy dưới 1 giây/CV không đồng nghĩa toàn bộ quy trình tuyển dụng kết thúc trong một giây, vì HR vẫn phải kiểm tra bằng chứng và chịu trách nhiệm quyết định. Điều khó nhất khi viết Problem Statement là tách metric kỹ thuật khỏi impact thật đối với HR và đặt boundary đủ rõ cho một bài toán tuyển dụng. Đóng góp rõ nhất của tôi là tổng hợp và viết lại Problem Statement v0 thành v1, trong đó giới hạn pilot vào một vị trí và yêu cầu mọi claim phải truy được về CV gốc. Tôi cũng thay đổi quan điểm từ việc coi multi-agent là đích đến sang xem nó là một thành phần có giới hạn bên trong workflow. Research giúp tôi thấy nhóm không cần tự xây OCR từ đầu, nhưng tài liệu sản phẩm không thể thay thế validation với người dùng thật. Tôi đồng ý với quyết định Not Yet vì nhóm chưa có baseline HR, CV ẩn danh và benchmark có thể tái lập. Nếu làm lại, tôi sẽ challenge việc đổi actor từ ứng viên sang HR sớm hơn và phỏng vấn HR trước khi chốt kiến trúc multi-agent.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

