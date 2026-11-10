# 주소한눈 (jusohannun)

행정안전부 도로명주소 API 기반 모바일 웹앱.

## 배포
GitHub 저장소 Settings > Pages > Source를 GitHub Actions로 설정합니다.
배포 URL: https://softm.github.io/jusohannun/

## 공식 주소 API
1. https://business.juso.go.kr/ 에서 검색 API 승인키 발급
2. Cloudflare Workers: `cd worker && npx wrangler deploy`
3. 비밀키 등록: `npx wrangler secret put JUSO_API_KEY`
4. 웹앱 API 설정에 Worker HTTPS URL 입력

공개 저장소에 API 키를 올리지 마세요. API가 미설정된 경우 검색은 동작하지 않습니다.
최근 검색과 즐겨찾기는 로컬 저장소에 저장됩니다.
