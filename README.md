# 🔋 BMS 电池数据记录器

通过上传 BMS App 截图，自动 OCR 提取电池数据并记录，支持导出 CSV。

## 部署到 GitHub Pages

1. 在 GitHub 创建新仓库（如 `bms-logger`）
2. 把 `index.html` 上传到仓库根目录
3. 进入仓库 **Settings → Pages**
4. Source 选择 `Deploy from a branch`，Branch 选 `main`，目录选 `/（root）`
5. 保存后等约 1 分钟，访问 `https://<你的用户名>.github.io/bms-logger/`

## 功能

- 📸 上传 BMS 截图（充电/放电/静置均支持），AI 自动识别所有数据
- 🛣 手动填写里程表读数，可与截图一起记录或单独记录
- ⬇ 导出 CSV（带 BOM，Excel 直接打开无乱码）
- ⬆ 导入 CSV（支持合并，自动去重）
- 🗑 删除单条记录（有确认弹框）
- 📦 数据保存在浏览器 localStorage，关闭页面不丢失

## 识别字段

SOC%、充放电状态、剩余时间、总电压、电流、容量、剩余容量、
串数、化学体系、最高/最低单体电压、压差、各温度传感器、
充放电回路状态、所有单体电压、告警信息
