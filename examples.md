# MacroDroid Automation Examples  
Real-device verified automation recipes for Android

This document provides detailed explanations for each `.macro` file in this repository.  
All examples follow a consistent structure:

- Purpose（目的）
- Trigger（何をきっかけに動くか）
- Action（実行内容）
- Constraint（条件・誤作動防止）
- Logic（なぜこの構成なのか / 代替案）
- Notes（実機検証での注意点）
- OS Considerations（Androidバージョン差分）

---

# 📚 Example List

以下は、このリポジトリに含まれる MacroDroid マクロの一覧です。  
（※ `.macro` を追加したら、このリストに追記してください）

---

## 1. 自宅に入ったら Wi-Fi を自動 ON  
**File:** `wifi_auto_on.macro`

### **Purpose**
自宅に入った瞬間に Wi-Fi を自動で ON にする。

### **Trigger**
- ジオフェンス（自宅エリアに入ったとき）

### **Action**
- Wi-Fi ON

### **Constraint**
- 画面OFF時のみ（誤作動防止）

### **Logic**
- ジオフェンスは誤差があるため、  
  「画面OFF時のみ」で無駄な ON/OFF を防ぐ。
- Bluetooth や基地局トリガーより安定性が高い。

### **Notes**
- Android 10 以降は位置情報権限が必須。
- 省電力モード中は精度が落ちる。

### **OS Considerations**
- Android 12 以降：バックグラウンド制限の影響あり  
- Android 13：通知権限が必要（MacroDroid 全体）

---

## 2. イヤホン接続で Spotify を自動起動  
**File:** `spotify_auto_launch.macro`

### **Purpose**
イヤホンを接続したら Spotify を自動で起動する。

### **Trigger**
- Bluetooth 接続（イヤホン）

### **Action**
- Spotify アプリ起動

### **Constraint**
- 画面ON時のみ（誤作動防止）

### **Logic**
- Bluetooth 接続は誤検知があるため、  
  「画面ON時のみ」でユーザー操作と連動させる。

### **Notes**
- 一部メーカー（OPPO / Xiaomi）はバックグラウンド制限が強い。

### **OS Considerations**
- Android 14：バックグラウンドアプリ起動の制限が強化

---

## 3. 充電開始でサイレントモード解除  
**File:** `silent_off_on_charge.macro`

### **Purpose**
充電開始時にサイレントモードを解除する。

### **Trigger**
- 充電開始

### **Action**
- 音量を通常レベルに戻す

### **Constraint**
- 深夜帯は除外（誤作動防止）

### **Logic**
- 充電開始はユーザーの「帰宅」や「作業開始」と連動しやすい。
- 深夜帯は不要なので除外。

### **Notes**
- 一部端末では「充電開始」トリガーが遅延することがある。

### **OS Considerations**
- Android 12：バッテリー最適化の影響を受けやすい

---

## 4. スマホの自動スクロール開始（2026-5-15）  
**File:** `スマホの自動スクロール開始（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/android-auto-scroll/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 5. スマホの自動スクロール解除（2026-5-15）  
**File:** `スマホの自動スクロール解除（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/android-auto-scroll/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 6. 連続した電源番号拒否（2026-5-15）  
**File:** `連続した電源番号拒否（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/macrodroid-call-restrictions/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 7. 特定電源番号の着信無音（2026-5-15）  
**File:** `特定電源番号の着信無音（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/macrodroid-call-restrictions/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 8. 特定の電源番号拒否（2026-5-15）  
**File:** `特定の電源番号拒否（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/macrodroid-call-restrictions/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 9. smsワンタイムパスワードの自動コピー（2026-5-15）  
**File:** `smsワンタイムパスワードの自動コピー（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/one-time-password-auto-save/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 10. イヤホンとSpotify連携の自動化（2026-5-15）  
**File:** `イヤホンとSpotify連携の自動化（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/auto-play/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 11. スマホ着信点滅の自動化（2026-5-15）  
**File:** `スマホ着信点滅の自動化（2026-5-15）.macro`  
**Article:** https://kamonomichi.com/smartphone-led/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 12. スマホ再起動の自動化（2026-5-15_Android16）  
**File:** `スマホ再起動の自動化（2026-5-15_Android16）.macro`  
**Article:** https://kamonomichi.com/smartphone-reboot/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 13. スマホ再起動の自動化（2026-5-15_Android12以前）  
**File:** `スマホ再起動の自動化（2026-5-15_Android12以前）.macro`  
**Article:** https://kamonomichi.com/smartphone-reboot/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 14. 位置情報ON-OFFの自動化（2026-5-13）  
**File:** `位置情報ON-OFFの自動化（2026-5-13）.macro`  
**Article:** https://kamonomichi.com/macrodroid-location-automation/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 15. 位置情報ON-OFFの自動化（2026-5-13）  
**File:** `位置情報ON-OFFの自動化（2026-5-13）.macro`  
**Article:** https://kamonomichi.com/macrodroid-amazon-music/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 16. Amazon_Musicカーナビ自動化（2026-5-13）  
**File:** `Amazon_Musicカーナビ自動化（2026-5-13）.macro`  
**Article:** https://kamonomichi.com/macrodroid-amazon-music/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 17. Androidテザリング自動化（root化なし2026-5-13）  
**File:** `Androidテザリング自動化（root化なし2026-5-13）.macro`  
**Article:** https://kamonomichi.com/android16-tethering-automation/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

## 18. Androidテザリング自動化（root化なし、トリガー1つ、2026-5-13）_  
**File:** `Androidテザリング自動化（root化なし、トリガー1つ、2026-5-13）_.macro`  
**Article:** https://kamonomichi.com/android16-tethering-automation/

### **Purpose**
TODO

### **Trigger**
- TODO

### **Action**
- TODO

### **Constraint**
- TODO

### **Logic**
- TODO

### **Notes**
- TODO

### **OS Considerations**
- TODO

---

# 🧠 Author

**Kamo**  
MacroDroid Specialist / Android Automation Expert  
https://kamonomichi.com/

---

# 📄 Notes

- `.macro` ファイルを追加したら、この `examples.md` に追記してください。
- すべての例は **実機検証済み** で、再現性を重視しています。