# Hoc Git

## Cach SetUp

Đây là một thẻ p thông thường

Tiếp theo là ul, li

- Đây là li
- Đây là li

[Đây là thẻ a](google.com)
![Đây là chó](./images.jpg)

**in đậm**
_in nghiêng_

> Đây là quoting

đây là `git bash`

```js
const a = 100;
```

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <p>Học git căn bản</p>
    <h3>TranNguyenHaiDang</h3>
    <h2>TranNguyenHaiDang</h2>
    <h1>TranNguyenHaiDang</h1>
    <h4>TranNguyenHaiDang</h4>
  </body>
</html>
```

```bash
git log
```

| header1  | header2  | header3  |
| -------- | -------- | -------- |
| content1 | content2 | content3 |
|          |          |          |
|          |          |          |

- git branch -r: hiển thị tất cả các nhánh trên remote
- git branch -a: hiển thị tất cả các nhánh dưới local và trên remote
- git branch: chỉ xem nhánh dưới local
- git switch -c <tên nhánh> = git checkout -b <tên nhánh>: tạo nhánh mới và chuyển sang nhánh mới
- git branch <tên nhánh>: chỉ tạo nhánh mới
- git branch -D <tên nhánh>: xóa nhánh dưới local
- git push origin --delete <tên nhánh>: xóa nhánh trên remote
- git checkout <tên nhánh> = git switch <tên nhánh>: chuyển nhánh
- git branch -m <tên nhánh>: đổi tên nhánh
- git fetch: lấy data mới nhất trên remote
- git push -u origin <tên nhánh>: đẩy nhánh dưới local lên remote mà không cần thay đổi nội dung trong nhánh đó
- git fetch -p : để cập nhật lại các branch đã bị xóa trên remote(dùng github để xóa)
- git push -u origin <tên nhánh>: lệnh push lần đầu để những lần push sau không cần viết tên nhánh nữa(git push)
- cat .git/config: để xem local branch đã kết nối với remote branch chưa
- git pull: là sự kết hợp giữa git fetch và git merge
- git merge <tên nhánh>: dùng để merge nhánh
- git merge --continue --no-edit: lấy message mặc định khi merge rồi mới push
- git checkout <tên file> = git restore <tên file>: dùng để khôi phục file lại trạng thái ban đầu khi đã thay đổi
- git reset <tên file> = git restore -S <tên file>: dùng để khôi phục file ở trạng thái staged(git add) thành trạng thái changes
- git restore --source=4b5c4d8 <tên file>: Tìm tên commit trong quá khứ và lấy nội dung đó ghi đè lên nội dung hiện tại
- git reset <mã hash> (mặc định là --mixed): đưa thay đổi về changes
- git reset --soft <mã hash>: đưa thay đổi về staged
- git reset --merge <mã hash>: giống --hard nhưng an toàn hơn, chỉ làm mất những thay đổi cần thiết
- git log --oneline: hiện ra lịch sử mã hash đã commit
- git push -f: ép đẩy lên
- git revert <mã hash> --no-edit: tạo ra một commit mới đối ngược với commit cũ
- git rebase -i HEAD~3(commit dòng 3): để gộp commit(gộp commit sau vào commit trước mới được) và thay đổi message cũ đã commit
- git rebase --abort: hủy rebase
- git commit --amend: thay đổi tên message hoặc logic của commit gần nhất(cuối cùng)
