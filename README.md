## 📸 Screenshots & Demonstration

### 1. Application Interface
![Main Interface](SQL_Injection_Defense.png)

---

### 2. Unsafe Mode vs. Safe Mode (`' OR '1'='1`)
Comparison of how the application handles the classic authentication bypass payload:

| ❌ Unsafe Mode (Vulnerable) | ✅ Safe Mode (Protected with PDO) |
| :--- | :--- |
| ![Unsafe Mode](unsafe%20mode.png) | ![Safe Mode](safe%20mode%20with%20OR%201=1.png) |
| **Result:** Query is manipulated and returns unauthorized user records. | **Result:** Payload is treated strictly as literal string data; injection is blocked. |
