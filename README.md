# Study Jam — Knowledge Hub

> Website lưu trữ, hệ thống hóa và chia sẻ kiến thức được học qua từng buổi Study Jam. Nội dung được bổ sung định kỳ hằng tuần để các thành viên có thể xem lại bài học, tra cứu tài liệu và tiếp tục tự học sau mỗi buổi.

## 1. Giới thiệu

**Study Jam Knowledge Hub** là website tài liệu học tập của Study Jam. Dự án hướng đến việc tập hợp kiến thức từ các buổi sinh hoạt thành một nguồn tham khảo chung, có cấu trúc và dễ truy cập.

Thay vì để kiến thức chỉ nằm trong slide hoặc tài liệu của từng buổi, website sẽ được cập nhật sau mỗi tuần để:

- Hệ thống hóa nội dung đã học theo từng chủ đề và từng buổi.
- Giúp thành viên xem lại kiến thức bất cứ lúc nào.
- Tập hợp slide, ghi chú, ví dụ, mã nguồn thực hành và tài liệu tham khảo.
- Tạo lộ trình học liên tục giữa các tuần.
- Giúp thành viên mới có thể tự tìm hiểu nội dung của những buổi trước.

## 2. Nội dung hiện có

Các tài liệu trong phiên bản hiện tại tập trung vào **Version Control, Git và GitHub**.

| Tài liệu | Nội dung |
|---|---|
| `version_control_and_git.docx` | Khái niệm Version Control; Local, Centralized (CVCS) và Distributed (DVCS); Git và các đặc điểm; Working Directory, Staging Area, Repository; cài đặt và cấu hình Git trên Windows. |
| `GITHUB.docx` | GitHub là gì; phân biệt Git và GitHub; Repository, Branch, Pull Request, Issues, GitHub Actions, Projects; giới thiệu GitLab và Bitbucket; quy trình cộng tác nhóm và demo GitHub cơ bản. |
| `index.html` | Website trình chiếu chủ đề Git & GitHub gồm 12 slide, có điều hướng bằng bàn phím/nút bấm, thanh tiến trình và bố cục responsive. |

### Các chủ đề đã được đề cập

- Tổng quan về quản lý phiên bản.
- Sự khác nhau giữa Local VCS, CVCS và DVCS.
- Git và quy trình làm việc với Working Directory, Staging Area, Local Repository và Remote Repository.
- Các lệnh Git cơ bản: `init`, `clone`, `status`, `add`, `commit`, `branch`, `pull`, `push`.
- GitHub và các tính năng hỗ trợ cộng tác.
- GitLab và Bitbucket như những nền tảng lưu trữ, cộng tác thay thế.
- Quy trình làm việc nhóm: Clone → Branch → Commit → Push → Pull Request → Review → Merge.

## 3. Truy cập website

Dự án hiện sử dụng HTML, CSS và JavaScript thuần; chưa cần cài đặt framework hay chạy lệnh build.

1. Clone hoặc tải repository về máy.
2. Mở thư mục dự án.
3. Mở file `index.html` bằng trình duyệt.

Có thể dùng Visual Studio Code và tiện ích Live Server để chạy website trên máy local.

```bash
git clone <repository-url>
cd <repository-folder>
```

Sau đó mở `index.html` hoặc chọn **Open with Live Server** trong VS Code.

## 4. Cấu trúc thư mục

Cấu trúc hiện tại:

```text
study_jam-main/
├── README.md
├── index.html
├── GITHUB.docx
└── version_control_and_git.docx
```

Khi nội dung tăng lên qua từng tuần, có thể tổ chức tài liệu theo cấu trúc thống nhất sau (đây là cấu trúc định hướng, không phải các thư mục đã có sẵn trong phiên bản hiện tại):

```text
study_jam/
├── README.md
├── index.html
├── assets/
│   ├── images/
│   └── files/
└── study-sessions/
    ├── week-01/
    │   ├── README.md
    │   ├── slides/
    │   ├── notes/
    │   └── resources.md
    ├── week-02/
    │   ├── README.md
    │   ├── slides/
    │   ├── notes/
    │   └── resources.md
    └── ...
```

## 5. Quy trình cập nhật sau mỗi buổi Study Jam

Mỗi tuần, người phụ trách nội dung có thể thực hiện theo quy trình sau:

1. **Thu thập tài liệu:** nhận slide, ghi chú, ví dụ, bài thực hành và đường dẫn tham khảo từ buổi học.
2. **Kiểm tra nội dung:** đối chiếu tài liệu buổi học; làm rõ thuật ngữ và những phần cần giải thích thêm. Không tự bổ sung thông tin chưa được xác minh.
3. **Biên tập:** sắp xếp kiến thức theo trình tự dễ học; giữ lại ví dụ và nội dung thực hành quan trọng.
4. **Bổ sung nguồn tham khảo:** ưu tiên tài liệu chính thức, ghi rõ tên nguồn và đường dẫn.
5. **Cập nhật website:** thêm mục/bài học mới vào website, đồng thời giữ lại nội dung của các tuần trước.
6. **Kiểm tra:** mở website trên máy tính và điện thoại; kiểm tra liên kết, hình ảnh, mã lệnh và khả năng điều hướng.
7. **Đăng thay đổi:** commit và push lên repository để các thành viên có thể truy cập phiên bản mới.

### Mẫu thông tin cho mỗi tuần

Mỗi buổi nên có một trang hoặc một mục nội dung với các thông tin:

| Trường thông tin | Nội dung cần ghi |
|---|---|
| Tuần / Buổi | Số thứ tự hoặc tên buổi Study Jam |
| Chủ đề | Chủ đề chính của buổi học |
| Mục tiêu | Sau buổi học, thành viên cần hiểu hoặc thực hiện được điều gì |
| Nội dung | Các kiến thức chính, được chia thành từng phần |
| Thực hành | Ví dụ, bài tập, demo hoặc mã nguồn liên quan |
| Tài liệu | Slide, file đính kèm và ghi chú |
| Tham khảo | Đường dẫn tài liệu chính thức hoặc nguồn đã kiểm chứng |
| Cập nhật | Ngày cập nhật và người phụ trách (nếu có) |

## 6. Nguyên tắc biên soạn nội dung

Để website thực sự hữu ích cho việc truyền tải kiến thức, nội dung nên tuân theo các nguyên tắc:

- **Chính xác:** ưu tiên nội dung từ tài liệu buổi học và tài liệu chính thức; phân biệt rõ kiến thức gốc với phần giải thích bổ sung.
- **Dễ tiếp cận:** giải thích thuật ngữ trước khi sử dụng; hạn chế giả định người đọc đã có kiến thức nền.
- **Có ví dụ:** ưu tiên ví dụ ngắn, tình huống thực tế, sơ đồ quy trình và đoạn mã có thể thử lại.
- **Có hệ thống:** chia nội dung theo tuần, chủ đề và mức độ; liên kết các kiến thức có liên quan.
- **Có thể tự học:** mỗi bài nên có tài liệu tham khảo và gợi ý nội dung cần xem tiếp.
- **Duy trì lịch sử:** không ghi đè hoặc xóa nội dung các tuần cũ khi bổ sung bài mới; nếu sửa nội dung, cần giữ lịch sử thay đổi qua Git.

## 7. Tài liệu tham khảo

Các liên kết dưới đây là nguồn tham khảo chính thức để học và kiểm tra lại kiến thức thuộc chủ đề Git, GitHub và các nền tảng liên quan.

### Git và Version Control

- [Git — Official Documentation](https://git-scm.com/doc)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Installing Git on Windows](https://git-scm.com/install/win)
- [Pro Git — About Version Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- [Pro Git — First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

### GitHub

- [GitHub Docs](https://docs.github.com/)
- [Getting Started with Git](https://docs.github.com/en/get-started/learning-to-code/getting-started-with-git)
- [About Git](https://docs.github.com/en/get-started/using-git/about-git)
- [GitHub — Hello World](https://docs.github.com/en/get-started/using-github/hello-world)
- [About Pull Requests](https://docs.github.com/en/pull-requests/get-started/about-pull-requests)
- [Git and GitHub Learning Resources](https://docs.github.com/en/get-started/start-your-journey/git-and-github-learning-resources)

### GitLab và Bitbucket

- [GitLab — Get Started](https://docs.gitlab.com/user/get_started/)
- [GitLab — Get Started with Git](https://docs.gitlab.com/topics/git/get_started/)
- [Bitbucket Cloud — Get Started](https://support.atlassian.com/bitbucket-cloud/docs/get-started-with-bitbucket-cloud/)
- [Bitbucket Cloud — Resources](https://support.atlassian.com/bitbucket-cloud/resources/)

> Khi thêm tài liệu cho các Study Jam tiếp theo, hãy bổ sung nguồn tham khảo đúng với chủ đề của buổi học; ưu tiên trang tài liệu chính thức và kiểm tra liên kết trước khi đăng.

## 8. Đóng góp và cập nhật

Mọi thành viên có thể đóng góp bằng cách bổ sung ghi chú, ví dụ, bài thực hành hoặc tài liệu tham khảo theo quy trình làm việc nhóm.

```bash
# Lấy phiên bản mới nhất
git pull

# Tạo nhánh cho phần nội dung cần cập nhật
git switch -c docs/week-XX-topic

# Sau khi chỉnh sửa, kiểm tra thay đổi
git status
git diff

# Đưa thay đổi vào staging và tạo commit
git add .
git commit -m "docs: add Study Jam week XX materials"

# Đẩy nhánh lên remote
git push -u origin docs/week-XX-topic
```

Sau đó tạo Pull Request để người phụ trách kiểm tra nội dung trước khi merge vào nhánh chính.

### Gợi ý quy ước commit

| Loại thay đổi | Prefix | Ví dụ |
|---|---|---|
| Thêm nội dung học tập | `docs:` | `docs: add Git basics session` |
| Cập nhật website | `feat:` | `feat: add weekly study navigation` |
| Sửa lỗi hiển thị/nội dung | `fix:` | `fix: correct Git command example` |
| Cập nhật tài nguyên | `assets:` | `assets: add session diagrams` |

## 9. Định hướng phát triển

Các hướng có thể triển khai khi số lượng buổi học tăng lên:

- Trang tổng quan liệt kê các buổi Study Jam theo tuần.
- Bộ lọc hoặc tìm kiếm theo chủ đề.
- Trang nội dung riêng cho từng buổi.
- Khu vực tải slide, tài liệu và mã nguồn thực hành.
- Mục bài tập / câu hỏi ôn tập sau mỗi chủ đề.
- Liên kết giữa bài học hiện tại và kiến thức nền cần xem trước.

Các mục trên là định hướng phát triển, không phải tính năng đã hoàn thành trong phiên bản hiện tại.

---

**Study Jam Knowledge Hub** — Học cùng nhau, lưu lại kiến thức, và tiếp tục phát triển mỗi tuần.
