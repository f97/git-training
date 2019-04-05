## [Rikkeisoft] Git Training

- Hướng dẫn về Git cơ bản cho người mới bắt đầu: Đọc ở [đây](http://backlogtool.com/git-guide/vn/intro/intro1_1.html) (Tiếng Việt), chú ý đọc cả phần **Nhập môn** và **Phát triển**.
- Sổ tay về Git: Đọc ở [đây](http://hnq90.github.io/git-guide/index.vi.html) hoặc [đây](https://learnxinyminutes.com/docs/vi-vn/git-vi/) (Tiếng Việt)
- Thực hành những thao tác căn bản với Git online: [Try Git](http://try.github.com/)  (Tiếng Anh)
- Những lệnh hay dùng: [Git Cheatsheet](http://www.git-tower.com/blog/git-cheat-sheet/)  (Tiếng Anh)
- Ebook hướng dẫn Git từ căn bản đến nâng cao: [Tiếng Anh](https://git-scm.com/book/en/v2) (updated 2014), [Tiếng Việt](https://git-scm.com/book/vi/v1) (updated 2009)
- Hướng dẫn sử dụng Git trên Netbean IDE: Đọc ở [đây](https://netbeans.org/kb/docs/ide/git.html)
- [Start a new git repository](http://kbroman.org/github_tutorial/pages/init.html)

## Git Client
Dưới đây là những phần mềm tương tác với Git qua giao diện đồ hoạ:
- [Github Desktop](https://desktop.github.com/) (Windows, Mac)
- [SourceTree](http://www.sourcetreeapp.com/) (Windows, Mac)
- [GitKraken](https://www.gitkraken.com/) (Windows, Mac, Linux)
- [GitExtension](https://github.com/gitextensions/gitextensions/releases) (Windows, Mac, Linux)
- [git-cola](http://git-cola.github.com/) (Windows, Linux)

## Cài đặt Git
- Windows: [Download](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C3%A0i-%C4%90%E1%BA%B7t-Git#Cài-Đặt-Trên-Windows)
- Linux: [Download](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C3%A0i-%C4%90%E1%BA%B7t-Git#Cài-Đặt-Trên-Linux)
- Mac: [Download](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C3%A0i-%C4%90%E1%BA%B7t-Git#Cài-Đặt-Trên-Mac)

## Cấu hình Git căn bản
Thiết lập thông tin cá nhân cho Git: (Sử dụng Git Bash hoặc Terminal để gõ các lệnh sau) **bắt buộc**
- `git config --global user.name "Ten cua ban"`
- `git config --global user.email <email rikkeisoft>`

- `git config --global core.safecrlf true`
- `git config --global color.ui true`
- `git config --global core.filemode false`

- `git config --global core.autocrlf input` (Cho Linux - Mac)
- `git config --global core.autocrlf true` (Cho Windows)

### Trường hợp code trên Windows nhưng chạy trên Linux
*Trong trường hợp code trên Windows nhưng code được đưa lên môi trường thực thi Linux bằng cách share folder hoặc upload trực tiếp, cần đảm bảo các file ở working copy có line endings kiểu Unix (LF) để chạy đúng trên môi trường Linux.*

Với các dự án này thì thực hiện config giống như trên môi trường Linux. Chú ý chỉ config cho riêng từng repository, không config global để tránh ảnh hưởng tới các repository có môi trường khác.
- `git config core.safecrlf true`
- `git config core.eol lf`
- `git config core.autocrlf input`
- Khi lưu file, cần chú ý file được lưu với line ending là LF (Có thể dùng plugin **Show and change line endings** của Netbeans để thay đổi line ending)

## Những điều chú ý khi dùng Git
- Viết nội dung commit có ý nghĩa và liên quan tới công việc đang làm.
 + Ví dụ: Issue #69, có yêu cầu: *"Viết chức năng đăng ký user cho hệ thống"* thì khi commit nên viết message là: **"Issue #69 Implement user registration feature"**

## Tip
- Bị lỗi liên quan đến line-ending:
```
git rm .gitattributes
git add -A
git reset --hard
```

## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
