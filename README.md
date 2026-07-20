### Soojung Choi — Portfolio (Static Site)

-  구조
```
portfolio_site/
├─ index.html            # 메인 원페이지
├─ style.css             # 공용 스타일 (미니멀 아카데믹)
├─ projects/             # 프로젝트 상세 페이지 13개
├─ assets/               # 프로필 사진 + 프로젝트별 이미지
├─ build_details.py      # (배포 불필요) 노션 md → 상세 HTML 변환 스크립트
└─ README.md
```
> `build_details.py`, `README.md`는 사이트 동작에 필요 없습니다. 올려도 무방하지만 빼도 됩니다.

- 로컬 미리보기
`index.html` 열기 

- GitHub Pages 배포 (username.github.io)
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
