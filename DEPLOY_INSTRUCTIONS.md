# Hướng dẫn Deploy lên GitHub Pages

## Bước 1: Push code lên GitHub

Bạn cần push code lên GitHub. Có 2 cách:

### Cách A: Sử dụng GitHub CLI hoặc đăng nhập lại
```bash
# Nếu bạn là chủ sở hữu repo (bvd0101), hãy đảm bảo đã đăng nhập đúng tài khoản
git push origin main
```

### Cách B: Sử dụng Personal Access Token
1. Vào GitHub.com → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Tạo token mới với quyền `repo`
3. Khi push, sử dụng token làm password:
```bash
git push origin main
# Username: bvd0101 (hoặc username của bạn)
# Password: [paste token của bạn]
```

## Bước 2: Bật GitHub Pages

1. Vào repository trên GitHub: https://github.com/bvd0101/giang_sinh_an_lanh
2. Click vào tab **Settings** (ở menu trên cùng)
3. Scroll xuống phần **Pages** (ở sidebar bên trái)
4. Trong phần **Source**, chọn:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

## Bước 3: Chờ và lấy link

- GitHub sẽ mất vài phút để build và deploy
- Sau khi xong, bạn sẽ có link: `https://bvd0101.github.io/giang_sinh_an_lanh/`
- Link này sẽ tự động cập nhật mỗi khi bạn push code mới lên branch `main`

## Lưu ý

- Nếu file không load được (ảnh, audio), có thể do tên thư mục có ký tự đặc biệt
- Trong trường hợp đó, bạn có thể cần đổi tên thư mục "Mê Ry Chí Mớt" thành tên không có dấu
- Hoặc di chuyển các file media lên root và cập nhật đường dẫn trong index.html

