# AbsoluteEye

<p align="right">
  <a href="https://github.com/sponsors/iahrung"><img src="https://img.shields.io/badge/❤️_Sponsor-iahrung-ea4aaa?style=flat-square&logo=github-sponsors" alt="Sponsor"></a>
  <img src="https://img.shields.io/badge/Platform-Windows-blue?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Year-~2000s–2020s-orange?style=flat-square" alt="Year">
  <img src="https://img.shields.io/badge/Category-RAT%20|%20Remote%20Access%20Trojan-red?style=flat-square" alt="Category">
</p>

> **🔑 Archive password / Mật khẩu giải nén:** `infected`
> **⚠️ Research & education use only / Chỉ dành cho nghiên cứu & giáo dục**

![Screenshot](https://raw.githubusercontent.com/iahrung/Ultimate-RAT/refs/heads/main/AbsoluteEye/Screenshot.png)

---

## 🇬🇧 English

### Overview

| Field | Value |
|---|---|
| **Name** | AbsoluteEye |
| **Platform** | Windows |
| **Language** | .NET / C++ / Delphi |
| **Category** | RAT / Remote Access Trojan |
| **First seen** | ~2000s–2020s |

**Description:**
AbsoluteEye is a .NET / C++ / Delphi-based Remote Access Trojan targeting Windows systems. Archived in this collection for security research, reverse engineering, and historical documentation of attacker tooling.

### Features

- Remote shell
- File manager
- Keylogger
- Screen capture
- Process manager
- Registry editor
- Persistence
- Password recovery

### 🛡️ White-Hat / Defensive Use

Analyze AbsoluteEye in a fully isolated VM/sandbox environment. Extract the archive (password: `infected`), open in dnSpy (if .NET) or x64dbg/Ghidra (if native). Set up a local listener on loopback, monitor with Wireshark, and build YARA/Sigma detection rules.

**Recommended setup:**
1. Install [FlareVM](https://github.com/mandiant/flare-vm) or a clean Windows VM (snapshot before analysis)
2. Extract archive: password `infected`
3. Open builder binary in **[dnSpy](https://github.com/dnSpy/dnSpy)** (for .NET) or **[x64dbg](https://x64dbg.com/)** (for native)
4. Set up a local listener on the default port (loopback only — `127.0.0.1`)
5. Monitor with **Wireshark** (capture C2 traffic) + **Process Monitor** (file/registry activity)
6. Build YARA / Sigma rules from observed patterns

### ⚔️ Threat Actor Context (Red Team / Pentest Reference)

AbsoluteEye is archived for historical documentation and security research. Understanding its capabilities helps defenders build detections and incident responders recognize its artifacts.

> **Legal reminder:** Only test against systems you own or have explicit written authorization to test. Unauthorized use is a criminal offense.

### 🔍 Indicators of Compromise (IoC)

Refer to sandbox reports on ANY.RUN, MalwareBazaar, and VirusTotal for current IoCs. Search Malpedia for 'AbsoluteEye' for actor attribution and detection rules.

### 📚 References

- https://malpedia.caad.fkie.fraunhofer.de/
- [Malpedia](https://malpedia.caad.fkie.fraunhofer.de/) — malware family database
- [ANY.RUN](https://any.run/) — interactive sandbox analysis

---

## 🇻🇳 Tiếng Việt

### Tổng quan

| Trường | Giá trị |
|---|---|
| **Tên** | AbsoluteEye |
| **Nền tảng** | Windows |
| **Ngôn ngữ** | .NET / C++ / Delphi |
| **Phân loại** | RAT / Remote Access Trojan |
| **Xuất hiện lần đầu** | ~2000s–2020s |

**Mô tả:**
AbsoluteEye là một Remote Access Trojan dựa trên .NET / C++ / Delphi nhắm mục tiêu hệ thống Windows. Được lưu trữ trong bộ sưu tập này để nghiên cứu bảo mật, reverse engineering và tài liệu hóa lịch sử công cụ tấn công.

### Tính năng

- Shell từ xa
- Quản lý file
- Keylogger
- Chụp màn hình
- Quản lý tiến trình
- Chỉnh sửa registry
- Persistence
- Khôi phục mật khẩu

### 🛡️ Sử dụng mũ trắng / Phòng thủ

Phân tích AbsoluteEye trong môi trường VM/sandbox hoàn toàn cô lập. Giải nén archive (mật khẩu: `infected`), mở trong dnSpy (nếu .NET) hoặc x64dbg/Ghidra (nếu native). Dựng listener local trên loopback, theo dõi bằng Wireshark và xây dựng rules YARA/Sigma.

**Môi trường đề xuất:**
1. Cài [FlareVM](https://github.com/mandiant/flare-vm) hoặc VM Windows sạch (tạo snapshot trước khi phân tích)
2. Giải nén archive: mật khẩu `infected`
3. Mở binary builder trong **[dnSpy](https://github.com/dnSpy/dnSpy)** (cho .NET) hoặc **[x64dbg](https://x64dbg.com/)** (cho native)
4. Dựng listener local trên cổng mặc định (chỉ loopback — `127.0.0.1`)
5. Theo dõi bằng **Wireshark** (bắt lưu lượng C2) + **Process Monitor** (hoạt động file/registry)
6. Xây dựng YARA / Sigma rules từ các pattern quan sát được

### ⚔️ Bối cảnh tác nhân đe dọa (Tham khảo Red Team / Pentest)

AbsoluteEye được lưu trữ để tài liệu hóa lịch sử và nghiên cứu bảo mật. Hiểu các khả năng của nó giúp người phòng thủ xây dựng phát hiện và ứng phó sự cố nhận ra dấu vết của nó.

> **Nhắc nhở pháp lý:** Chỉ kiểm thử trên hệ thống bạn sở hữu hoặc có văn bản cho phép kiểm thử. Sử dụng trái phép là vi phạm pháp luật hình sự.

### 🔍 Chỉ số xâm phạm (IoC)

Tham khảo báo cáo sandbox trên ANY.RUN, MalwareBazaar và VirusTotal để có IoC hiện tại. Tìm kiếm 'AbsoluteEye' trên Malpedia để có thông tin quy kết tác nhân và rules phát hiện.

### 📚 Tài liệu tham khảo

- https://malpedia.caad.fkie.fraunhofer.de/
- [Malpedia](https://malpedia.caad.fkie.fraunhofer.de/) — cơ sở dữ liệu họ malware
- [ANY.RUN](https://any.run/) — phân tích sandbox tương tác


## Archive

| Tool | Archive | Screenshot |
|---|---|---|
| AbsoluteEye | `Absolute®Eye v3.0.0.0 Fixed Version.7z` | [🖼](https://raw.githubusercontent.com/iahrung/Ultimate-RAT/refs/heads/main/AbsoluteEye/Screenshot.png) |

---

<sub>Lưu trữ bởi / Archived by <a href="https://github.com/iahrung">@iahrung</a> (Thu Hương) · <a href="https://github.com/sponsors/iahrung">Tài trợ / Sponsor ❤️</a> · <a href="https://github.com/iahrung/Ultimate-RAT">Ultimate-RAT Collection</a></sub>
