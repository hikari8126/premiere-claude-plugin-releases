# Premiere Claude Plugin — Releases

Kho **bản tải** cho Premiere Claude Plugin (file `.ccx` + `.zip` cài đặt).
Source code nằm ở repo riêng (private). Repo này chỉ giữ các bản release để đồng nghiệp tải về mà không cần đăng nhập.

## Cài đặt — một lệnh

Mở app **Terminal** trên Mac, dán lệnh này rồi Enter:

```bash
curl -fsSL https://raw.githubusercontent.com/hikari8126/premiere-claude-plugin-releases/main/install.sh | bash
```

Script tự cài Homebrew, Node.js, Claude CLI, ffmpeg, Whisper, **Claude Bridge** và plugin vào Premiere Pro
(bản mới nhất), rồi khởi động Bridge. Thứ gì máy đã có sẽ được bỏ qua.

Bạn chỉ cần:
- nhập **mật khẩu máy** nếu được hỏi (khi cài Homebrew),
- **đăng nhập Claude** trên trình duyệt khi nó mở ra (tài khoản Pro/Max).

Xong thì mở (hoặc khởi động lại) Premiere Pro → **Window → Extensions → Claude AI**.

Yêu cầu: macOS, Premiere Pro ≥ 25.6 và Creative Cloud Desktop.

Tuỳ chọn:
- Bỏ Whisper (~1GB, chỉ Autocut cần): `curl -fsSL ... | bash -s -- --no-whisper`
- Chỉ kiểm tra, không cài gì: `curl -fsSL ... | bash -s -- --dry-run`

Chạy lại cùng lệnh để cập nhật lên bản mới nhất.

## Cài thủ công

1. Vào [Releases](../../releases/latest) tải bản mới nhất.
2. Giải nén `.zip` → mở `Installer Claude AI.app` (chuột phải → Open).

Plugin tự kiểm tra bản mới và trỏ tới đây.
