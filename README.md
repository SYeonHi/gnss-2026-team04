# 2026-1 위성항법시스템 4팀

> SR로 만든 픽셀은 진짜 정보인가, 예쁜 환상인가? — RTK로 검증한다

## 개요
캠퍼스 5~6 스팟에서 두 점 A·B의 거리를 4가지 방법으로 측정해 비교한다:
1. 줄자 (mm급, 메타검증)
2. F9P PPK (±2cm, Ground Truth)
3. VWorld 원본 위성사진 픽셀 측정 환산
4. VWorld SR 사진 픽셀 측정 환산

## 팀원 / 역할
|  이름  |                  담당                   |
| 박소연 | F9P 운용, RTKLIB PPK, 분석, PM           |
| 정인욱 | VWorld 캡쳐, Real-ESRGAN SR, PSNR/SSIM  |
| 방지혜 | RasPi 로깅, 현장 운용                    |
| 이재덕 | 현장 보조, 픽셀 측정 도구, Folium 지도    |

## 폴더 구조
- `raw/` — F9P raw .ubx 로그 (3번)
- `rinex/` — CONVBIN 변환 결과
- `ngii_base/` — NGII RINEX 베이스 (1번)
- `vworld_orig/`, `vworld_sr/` — 위성 사진 (2번)
- `analysis/` — 4-way 비교, 그래프 (1번)
- `src/` — 모든 코드
- `docs/` — 발표 자료, 운용 매뉴얼

## 일정
- W1: 측정 인프라 + 본 측정
- W2: 후처리 + 분석 + 발표 준비
