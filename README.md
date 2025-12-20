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

git branch -r: hiển thị tất cả các nhánh trên remote
git branch -a: hiển thị tất cả các nhánh dưới local và trên remote
git branch: chỉ xem nhánh dưới local
git switch -c <tên nhánh> = git checkout -b <tên nhánh>: tạo nhánh mới và chuyển sang nhánh mới
git branch <tên nhánh>: chỉ tạo nhánh mới
git branch -D <tên nhánh>: xóa nhánh dưới local
git push origin --delete <tên nhánh>: xóa nhánh trên remote
git checkout <tên nhánh> = git switch <tên nhánh>: chuyển nhánh
git branch -m <tên nhánh>: đổi tên nhánh
git fetch: cập nhật lại dưới local khi thêm nhánh trên remote(dùng github để thêm)
git push -u origin <tên nhánh>: đẩy nhánh dưới local lên remote mà không cần thay đổi nội dung trong nhánh đó
git fetch -p : để cập nhật lại các branch đã bị xóa trên remote(dùng github để xóa)
git push -u origin <tên nhánh>: lệnh push lần đầu để những lần push sau không cần viết tên nhánh nữa(git push)
cat .git/config: để xem local branch đã kết nối với remote branch chưa
Handle B da edit
