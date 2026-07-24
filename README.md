# Portfolio

## Architecture
```
portfolio_site/
├─ index.html            # Main
├─ style.css             # 공용 스타일 (Minimal Academic style)
├─ projects/             # 프로젝트 상세 페이지 13개
├─ assets/               # 프로필 사진 + 프로젝트별 이미지
└─ README.md
```
## GitHub Pages 배포 (username.github.io)
1. GitHub에서 `<username>.github.io` 이름의 public 저장소 생성
2. 이 폴더의 **내용물**(index.html 등)을 저장소 루트에 push
   ```bash
   cd portfolio_site
   git init
   git add .
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```
3. 저장소 Settings → Pages → Branch: `main` / `/ (root)` → Save
4. 몇 분 뒤 `https://<username>.github.io` 에서 확인
