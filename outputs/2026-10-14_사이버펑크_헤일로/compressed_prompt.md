# 압축 프롬프트 재현 테스트

## 조건
- 기준 이미지: `13.png`
- 생성 이미지: `14_compact-prompt-test.png`
- 이미지 레퍼런스 없이 아래 압축 프롬프트만 사용

## 압축 프롬프트

```text
White-background 3:2 industrial prop design sheet, four consistent views. One complete vertical cyberpunk halo behind a head: a thin flat rectangular cable-tie band, not a tube. About 88% is warm yellow-orange light and 12% is a compact upper-right white/silver armored graphite hub. Two broad arcs (upper-left and bottom) glow through their entire flat width and thickness; their four endpoints use nonmatching irregular diagonal/wedge seams. Other arcs have silver edges around a recessed orange inlay.

A long slim orange-lit antenna rises diagonally from the hub. At its absolute root, squeezed against the housing with zero slack, a double-size pristine glossy white barcode tag is tied by one black loop; collision with the housing forces it upward/outward 40 degrees. Barcode bars only, no characters.

Three long lines sag in separate U-loops from hub to one round occipital pad: one thick frayed black braided cable, one thin red wire, one thin blue wire. Include front, rear, mannequin side-fit, and close details. Crisp hard-surface SF, flat neutral lighting.

Avoid text, logos, extra rings/wires/tags, open ring, round neon tube, bulky hub, regular perpendicular light boundaries, hair, clothing, scenery, watermark.
```

## 육안 비교
- 전체 콘셉트: 높음. 단일 폐쇄형 케이블타이 링, 백색·흑연색 허브, 주황 발광이 유지됨.
- 핵심 부품: 높음. 긴 안테나, 태그, 굵은 검정선, 얇은 빨강·파랑선, 뒤통수 패드가 모두 재현됨.
- 발광 구간: 중상. 전폭 발광 호와 사선 경계는 재현됐지만 기준 이미지의 네 경계 위치와 쐐기 모양이 정확히 같지는 않음.
- 태그 배치: 중간. 안테나 뿌리에는 있으나 기준 이미지처럼 허브에 눌려 위로 튀어 오른 느낌이 약함.
- 와이어 처짐: 중간. 세 종류는 구분되지만 기준 이미지보다 U자 처짐이 짧고 정돈됨.
- 허브 디테일: 중간. 크기와 색은 유사하나 장갑 패널과 소켓 구조가 단순화됨.
- 시트 구성: 중간. 다각도와 상세 뷰는 있으나 독립 오브젝트 중심인 기준 이미지보다 마네킹 비중이 커짐.

## 결론
- 형태·색상·부품 수준의 재현도: 약 75%.
- 세부 배치와 설정화 구성까지 포함한 재현도: 약 60~65%.
- 압축 프롬프트에 `긴 U자 처짐`, `태그 강제 들림`, `독립 오브젝트 3뷰 + 착용 1뷰`를 한 문장씩 보강하면 개선 가능.
# 압축 프롬프트 v2 — 안테나 방향·태그 크기 보정

```text
White-background 3:2 industrial prop sheet: isolated front and rear object views, one mannequin side-fit view, close details. One complete vertical cyberpunk halo, thin flat rectangular cable-tie band. About 88% warm orange light, 12% compact upper-right white/silver and graphite hub. Upper-left and bottom arcs glow across their full flat width; four endpoints have different irregular diagonal wedge seams. Other arcs have silver edges and recessed orange inlay.

A long slim antenna exits the hub at a 90-degree OUT-OF-PLANE angle, along the halo plane’s normal, pointing horizontally backward away from the wearer. It must not point upward within the ring plane: front view shows strong foreshortening, side view shows its full horizontal length. At the antenna’s absolute root, a huge pristine glossy white 9×4.5 cm barcode tag—larger than the hub—is cinched with zero slack and forced upward/outward by collision with the armor. Barcode bars only.

Three long separate U-loop connections run from hub to one occipital pad: thick frayed black braid, thin red wire, thin blue wire. Crisp hard-surface SF, neutral lighting. Avoid extra parts, open/round ring, upright in-plane antenna, small tag, readable text, hair, clothing, scenery, watermark.
```

## v2 무참조 재현 결과

- 결과: `15_compact-prompt-v2.png`
- 안테나는 링 평면 안에서 위로 서지 않고, 링 평면의 법선 방향으로 90도 꺾여 뒤쪽을 향하는 형태로 재현됨.
- 태그는 이전 압축 테스트보다 확실히 커지고 광택 있는 새 제품 재질이 유지됨. 다만 목표인 ‘허브보다 압도적으로 큼’은 아직 약함.
- 완전한 단일 링, 주황 발광, 사선형 발광 경계는 대체로 유지됨.
- 독립 소품 뷰에서 뒤통수 패드가 링 하단의 추가 기계 모듈처럼 합쳐졌고, 전선도 긴 U자 처짐보다 허브와 하단 모듈을 잇는 배선으로 변형됨.
- 추정 유사도: 핵심 구성·색상 약 70–75%, 세부 배치·와이어 구조 약 55–60%.

## 방향 용어

- 설계 지시: `링 평면의 법선 방향으로 90도 돌출`, 또는 `링 평면 밖으로 수평 돌출(out-of-plane)`.
- `외적`은 두 벡터로 법선 벡터를 구하는 연산이고, `내적`은 두 방향의 직교 여부를 확인하는 연산이므로 외형 지시어로는 쓰지 않는 편이 정확함.

