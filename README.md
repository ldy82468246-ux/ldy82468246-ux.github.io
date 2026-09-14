# ldy82468246-ux.github.io

이동윤 개인 홈페이지. 프레임워크 없이 HTML 한 장 + 데이터 파일 하나로 되어 있고, GitHub Pages로 배포됩니다.

## 파일

| 파일 | 역할 |
|---|---|
| `index.html` | 사이트 본체. `data.json`을 읽어서 화면을 그림 |
| `data.json` | **모든 내용** (프로필, 소개, 학력, 경력, 논문, 연락처). 이것만 고치면 됨 |
| `admin/index.html` | 관리 페이지. 폼으로 `data.json`을 편집하고 GitHub에 바로 저장 |
| `images/profile.jpg` | 프로필 사진 |
| `.nojekyll` | GitHub Pages가 Jekyll 처리를 건너뛰게 함 |

## 내용 수정하는 법

1. `https://leedongyun.com/admin/` 접속
2. 처음 한 번만 GitHub 토큰 연결 (페이지 안에 순서 안내가 있음)
3. 폼에서 고치고 **저장 · 배포** → 1~2분 뒤 사이트 반영

관리 페이지는 `data.json`을 GitHub API로 커밋하는 것뿐이라, GitHub 웹에서 `data.json`을 직접 고쳐도 똑같이 반영됩니다.

## 디자인·구조 수정

`index.html` 안의 `<style>`과 `render()` 함수를 고치면 됩니다. 로컬 확인은 아무 정적 서버로:

```bash
npx --yes serve .
```
