# 사이버펑크 헤일로 설정화

## 사용 파일
- 소품: `props/사이버펑크_헤일로.md`
- 스타일: 별도 스타일 파일 없음. 사용자 요청의 `금속 SF 사이버펑크` 방향을 소품 설정에 직접 반영.
- 1차 레퍼런스 이미지: 없음
- 추가 레퍼런스: 사용자가 대화에 첨부한 캐릭터 스케치. 캐릭터 자체가 아니라 머리 뒤 광륜의 실루엣과 구조만 참조.

## 1차 프롬프트

```text
Use case: stylized-concept
Asset type: production prop design reference sheet
Primary request: Create a clean multi-view design sheet of one consistent cyberpunk science-fiction halo device that floats vertically behind a character's head. Show the object alone, with no character or head.
Scene/backdrop: pure plain white studio background.
Subject: a thin circular halo with exactly eight evenly spaced curved metal segments forming one complete ring; eight narrow glowing gaps between the segments; outer diameter about 42 cm, ring width about 3 cm, thickness about 1.2 cm. The ring is vertical, never horizontal. Each segment has shallow fine circuit grooves with restrained cyan light. Inner edge contains a vivid cyan energy channel. Segment junctions contain compact black ceramic and dark chrome magnetic levitation nodes. A single small trapezoidal control module sits at bottom center, with exactly one tiny red status light.
Style/medium: high-end industrial design concept art, precise hard-surface sci-fi prop rendering, metallic cyberpunk aesthetic, crisp technical presentation without written annotations.
Composition/framing: landscape 3:2 sheet. Four clearly separated depictions of the exact same object: large front orthographic view, side orthographic view showing thin depth and slight backward curvature, rear orthographic view showing clean panel construction with no cables, and one close-up detail of a segment joint, levitation node, and cyan energy channel. Maintain identical proportions, component count, color placement, and details in every view.
Lighting/mood: even flat neutral studio lighting, highly legible form, minimal soft grounding shadows only.
Color palette: dark matte gunmetal titanium, subtle silver edge wear, black ceramic, dark chrome, vivid cyan emission, one tiny red indicator.
Materials/textures: brushed matte titanium panels, precise machined seams, restrained edge wear, smooth ceramic nodes.
Constraints: exactly eight metal segments in front and rear views; one bottom-center control module; clean white background; no text anywhere; no labels; no logos; no measurements; no human scale silhouette.
Avoid: character, person, face, head, hands, worn-on-body view, angel wings, sacred symbols, crown shapes, horizontal ring, cables, antennas, spikes, excessive ornament, background scenery, dramatic lighting, motion blur, typography, captions, watermark.
```

## 네거티브
- character, person, face, head, hands, worn-on-body view
- angel wings, sacred symbols, crown shapes
- horizontal ring, cables, antennas, spikes, excessive ornament
- background scenery, dramatic lighting, motion blur
- typography, captions, labels, measurements, logos, watermark

## 비율
- 가로 3:2

## 검수 결과
- 통과: 수직 원형 광륜 구조가 명확함.
- 통과: 정면 및 후면의 금속 세그먼트가 8개로 유지됨.
- 통과: 건메탈 외장, 청록색 에너지 채널, 하단 제어 모듈과 적색 상태등이 뷰 사이에서 일관됨.
- 통과: 측면 뷰에서 얇은 두께와 곡률이 읽힘.
- 통과: 흰 배경이며 인물, 손, 문자, 로고가 없음.
- 참고: 디테일 확대는 자기부상 노드와 에너지 채널을 선명하게 보여줌.

## 시도별 수정 내역
- 1차 생성: 완전한 8분절 원형 링으로 생성. 이후 제공된 스케치와 형태가 달라 폐기.
- 2차 생성: 첨부 스케치에 맞춰 3중 개방형 호와 우측 상단 허브 구조로 전면 수정. `02.png`로 채택.

## 최종 프롬프트 (2차)

```text
Use case: stylized-concept
Asset type: production prop design reference sheet
Input image: use the user's attached sketch montage only as the authoritative silhouette and placement reference for the halo apparatus behind the character. Extract and redesign only the halo apparatus; do not reproduce either character, the screenshot UI, or any other elements.
Primary request: Create a clean multi-view design sheet of the asymmetrical cyberpunk science-fiction halo shown in the sketch. It is a floating vertical apparatus for behind the head, made from three slender open metal orbital arcs attached to one angular mechanical hub near the upper-right side. It must preserve the sketch's distinctive sweeping, layered, incomplete-circle silhouette. This is not a complete circular ring.
Subject construction: exactly three thin parallel gunmetal tracks, each following a different radius, sweeping broadly around an empty head-sized central space. The tracks do not intersect and do not close into full circles. Their starts and ends gather around one compact angular mechanical hub at the upper-right. The hub has one short narrow radiator fin or rod rising diagonally upward, matching the sketch. Each track has a fine cyan illuminated line along its inner edge. The hub is black ceramic and dark chrome with restrained cyan circuit grooves and subtle silver edge wear.
Scene/backdrop: pure plain white studio background.
Style/medium: precise high-end hard-surface sci-fi industrial concept art, metallic cyberpunk prop rendering, clean and readable reference-sheet presentation.
Composition/framing: landscape 3:2 sheet. Show four separated depictions of the same apparatus: large front orthographic view emphasizing the three open sweeping arcs and upper-right hub; side orthographic view showing the layered depth and backward curvature; rear orthographic view showing the hub's rear panels and attachment of all three tracks; close-up detail of the angular hub, diagonal fin, and three track sockets. Keep the exact same silhouette, track count, hub position, proportions, and colors in every view.
Lighting/mood: neutral even flat studio lighting, crisp edges, only minimal soft grounding shadows.
Color palette: matte dark gunmetal titanium, black ceramic, dark chrome, cyan emission, subtle silver wear.
Constraints: exactly three open arcs; one hub at upper-right; one diagonal fin; open asymmetrical halo silhouette matching the input sketch; clean white background; no text, labels, dimensions, logos, or watermark.
Avoid: complete closed ring, thick segmented donut, circular disc, symmetric ring, character, person, face, head, hair, hands, clothing, screenshot interface, angel wings, sacred symbols, crown, cables, extra antennae, spikes, excessive decoration, scenery, dramatic lighting, motion blur.
```

## 최종 검수 결과
- 통과: 3개의 가느다란 개방형 금속 궤도가 모든 뷰에서 유지됨.
- 통과: 우측 상단 기계식 허브와 비스듬한 핀 1개가 유지됨.
- 통과: 완전한 원형 링이 아닌 비대칭 열린 광륜으로 표현됨.
- 통과: 건메탈과 청록색 발광선이 모든 뷰에서 일관됨.
- 통과: 인물, 손, 텍스트, 배경 장면이 없음.

## 3차 수정
- 사용자 수정: 륜을 3개에서 1개로 변경.
- 색상 레퍼런스: 사용자가 첨부한 백색 SF 메카 이미지에서 밝은 백색·은회색 장갑, 흑연색 내부 프레임, 노랑·주황 발광 패턴만 참조.
- 결과: `03.png`

### 최종 프롬프트 (3차)

```text
Use case: stylized-concept
Asset type: production prop design reference sheet
Input references: One reference shows the previous multi-view halo concept; use only its open asymmetrical sweep, upper-right hub placement, and diagonal fin, but REDUCE the construction to exactly ONE arc. The other reference is a white science-fiction mechanical creature image; use it only for the metal color blocking and surface language: bright white and pale silver angular armor plates, dark graphite recessed structure, and warm yellow-to-orange emissive seams. Do not reproduce the creature, its logo, text, composition, or background.
Primary request: Create a clean multi-view design sheet of one asymmetrical cyberpunk science-fiction halo apparatus floating vertically behind a head. The halo has EXACTLY ONE slender open metal arc attached to one compact angular hub at the upper-right. ONE ARC ONLY. No parallel rings, no nested arcs, no second orbit.
Construction: one broad C-shaped open arc sweeping around an empty head-sized central space, with both ends associated with the compact upper-right mechanical hub region. The halo is incomplete and asymmetrical, not a full closed circle. The upper-right hub has one short narrow fin rising diagonally upward. The arc is about 1.4 cm wide with layered angular armor plating.
Color/material design: predominantly bright matte white armor with pale silver facets; visible dark graphite mechanical structure in panel gaps and underside; restrained warm golden-yellow to orange light glowing through thin recessed seams along the inner edge and hub. No cyan, blue, teal, green, red, or purple light.
Scene/backdrop: pure plain white background.
Style/medium: precise high-end hard-surface science-fiction industrial concept art, clean production reference sheet, crisp mechanical panel design.
Composition/framing: landscape 3:2. Four clearly separated depictions of the exact same object: large front orthographic view, side orthographic view showing thin depth and gentle backward curvature, rear orthographic view showing dark recessed framework, and close-up of the upper-right hub plus arc joint. Every depiction must have exactly one open arc, one upper-right hub, and one diagonal fin. Preserve identical proportions and color placement.
Lighting: even neutral flat studio lighting, highly legible, minimal soft grounding shadow.
Constraints: EXACTLY ONE C-SHAPED OPEN ARC in every view; one upper-right hub; one diagonal fin; white/silver armor, graphite recesses, yellow-orange emissive seams; clean white background; no characters, head, hands, text, labels, measurements, logos, or watermark.
Avoid: multiple arcs, double ring, triple ring, nested rings, parallel tracks, complete closed ring, thick donut, circular disc, symmetric halo, cyan, blue or teal illumination, creature, dragon, person, hair, clothing, screenshot interface, typography, angel wings, sacred symbols, crown, cables, extra antennae, spikes, scenery, dramatic lighting, motion blur.
```

### 3차 검수
- 통과: 모든 뷰에서 륜이 정확히 1개임.
- 통과: 개방형 C자 실루엣과 우측 상단 허브가 유지됨.
- 통과: 백색·은회색 장갑, 흑연색 내부, 노랑·주황 발광이 일관됨.
- 통과: 청록색 발광, 캐릭터, 문자, 로고가 없음.

## 4차 수정
- 사용자 수정: 링을 끊김 없는 완전한 원으로 변경.
- 구성 비율: 둘레 약 80%는 노랑·주황 발광 에너지 링, 약 20%는 우측 상단의 백색 기계장치.
- 구분 방식: 발광부 양끝을 기계장치의 소켓에 연결하여 두 영역의 경계를 명확히 함.
- 결과: `04.png`

### 최종 프롬프트 (4차)

```text
Use case: stylized-concept
Asset type: production prop design reference sheet
Input references: use the previous white/orange halo concept as the geometry and material starting point, and use the white science-fiction mecha reference only for white/silver armor, graphite recesses, and warm yellow-orange emission. Correct the previous open C-shape into one complete unbroken circular ring.
Primary request: Create a clean multi-view design sheet of exactly ONE complete circular cyberpunk halo that floats vertically behind a head. The ring must be a perfect, fully closed, unbroken circle. Approximately 80% of its circumference is a visibly luminous energy ring; the remaining approximately 20% is a compact mechanical apparatus integrated at the upper-right. Make the luminous region and the mechanical region visually unmistakable as two different functional zones.
Geometry: one continuous circular ring only. No gap anywhere. The 80% luminous portion is a smooth narrow energy conduit forming most of the circle, with a bright warm golden-yellow core and soft orange outer glow. It should look luminous rather than covered in armor. The 20% mechanical portion occupies one contiguous arc at the upper-right: layered bright white and pale silver angular armor plates over dark graphite internal machinery, including one short narrow radiator fin rising diagonally upward. Two precise socket transitions connect the ends of the 80% energy conduit into the 20% mechanical arc, completing the circle without interruption.
Color/material design: luminous region is golden yellow to warm orange energy; mechanical region is matte white and pale silver armor with dark graphite recesses and restrained orange light in seams. The mechanical armor must not extend around the rest of the ring. No cyan, blue, teal, green, red, or purple light.
Scene/backdrop: pure plain white background.
Style/medium: high-end hard-surface science-fiction industrial concept art, clean production reference sheet, precise mechanical panel design.
Composition/framing: landscape 3:2. Four separated depictions of the exact same object: large front orthographic view that clearly shows a fully closed circle and the 80:20 luminous-to-mechanical ratio; side orthographic view; rear orthographic view; close-up of one transition socket between luminous ring and mechanical apparatus. Preserve the same circle, ratio, hub position, fin, proportions, and colors in every view.
Lighting: neutral even flat studio lighting, crisp legibility, minimal soft shadow.
Hard constraints: exactly one ring; perfectly closed full circle; zero gaps; approximately 80% exposed glowing energy conduit; approximately 20% upper-right mechanical apparatus; strong visible boundary between glowing region and machine region; one diagonal fin; no metal cladding across the 80% luminous region; no text, labels, logos, measurements, character, head, hands, or watermark.
Avoid: open ring, C-shape, broken circle, multiple rings, nested rings, parallel tracks, mostly armored circumference, evenly distributed armor panels, thick donut, disc, cyan or blue glow, creature, person, hair, clothing, screenshot UI, typography, wings, sacred symbols, crown, cables, extra antennae, spikes, scenery, dramatic lighting, motion blur.
```

### 4차 검수
- 통과: 정면과 후면에서 단일 링이 끊김 없는 완전한 원을 이룸.
- 통과: 발광 영역이 둘레 약 80%, 기계장치 영역이 약 20%로 읽힘.
- 통과: 소켓 구조로 발광 영역과 기계장치 영역이 명확히 구분됨.
- 통과: 백색·은회색 장갑, 흑연색 내부, 노랑·주황 발광 패턴이 일관됨.

## 5차 수정
- 사용자 수정: 링을 원통형 레이저가 아닌 케이블타이 같은 물리적 금속 밴드로 변경.
- 구조: 폭 1.6cm, 두께 0.3cm의 납작한 직사각형 단면. 앞면의 약 80% 구간에 발광 인레이가 매입됨.
- 결과: `05.png`

### 최종 프롬프트 (5차)

```text
Use case: stylized-concept
Asset type: production prop design reference sheet
Input image role: edit/reference target. Preserve the single complete circle, upper-right white mechanical hub, diagonal fin, white/silver/graphite palette, and warm orange emission. Correct only the construction of the ring body: it must no longer look like a round laser tube.
Primary request: Redesign the complete circular cyberpunk halo as a thin, flat, cable-tie-like metal band. The entire ring is a physical solid strap with a flat rectangular cross-section, about 1.6 cm wide and only 0.3 cm thick. It bends into one perfect closed circle. It must look like a futuristic metallic zip tie or spring-steel band, not a beam of light, pipe, cable, hose, neon tube, or torus.
Ring construction: the band has opaque matte white and pale silver metal edges and an opaque dark graphite backside. Approximately 80% of the circumference has a broad, flat golden-yellow to warm-orange emissive inlay recessed into the center of the band’s FRONT FACE. This glow is a surface strip inside the physical band, not the entire ring material. The flat metal edges remain clearly visible around the glowing inlay. In side view, show the very thin rectangular sheet profile and zero tubular curvature.
Mechanical zone: the remaining approximately 20% at the upper-right is a compact, clearly separate cable-tie-lock-like mechanical housing: layered angular white/silver armor over dark graphite mechanics, with two flat strap sockets and one short diagonal radiator fin. The metal band passes into and out of this locking housing, completing the circle without gaps.
Scene/backdrop: pure plain white background.
Style/medium: precise high-end hard-surface science-fiction industrial concept art, clean production reference sheet.
Composition/framing: landscape 3:2 with four separated views of the exact same object: front orthographic view showing one closed circle and the 80:20 surface-light-to-machine ratio; strict side view emphasizing the flat thin sheet profile; rear view showing the opaque graphite backside with minimal light leakage; close-up of the flat band entering the mechanical lock housing. Maintain identical geometry and color placement.
Hard constraints: exactly one fully closed circular band; cable-tie silhouette; flat rectangular cross-section; solid physical metal strap visible through the full circumference; 80% front-face emissive inlay; 20% upper-right lock housing; visible white/silver borders around the glow; no gaps; no tubular ring.
Avoid: laser ring, pure-energy ring, neon tube, glowing rod, round cross-section, pipe, hose, electrical cable, torus, transparent ring, multiple rings, open C-shape, cyan or blue glow, character, head, hands, text, labels, logos, dimensions, watermark, scenery, dramatic lighting.
```

### 5차 검수
- 통과: 정면에서 발광 인레이 바깥으로 금속 밴드의 테두리가 보임.
- 통과: 측면에서 얇고 납작한 판형 단면이 확인됨.
- 통과: 후면은 불투명한 흑연색 금속 밴드로 표현됨.
- 통과: 완전한 원, 약 80% 발광 표면, 약 20% 기계식 잠금 허브가 유지됨.

## 승인 베이스 백업
- 사용자가 5차 디자인을 마음에 든다고 확인하여 `backup/05_approved-base.png`로 별도 보존.
- 소품 상태는 추가 수정 중이므로 `초안` 유지.

## 6차 수정
- 기계식 허브 뒤쪽에 거칠고 닳은 꼬임 와이어 1가닥 추가.
- 와이어 끝에 문자와 숫자 없이 검은 세로 막대만 있는 바코드 태그 1개 추가.
- 승인 베이스의 링 형태, 80:20 비율, 색상과 재질은 유지.
- 결과: `06.png`

### 최종 프롬프트 (6차)

```text
Use case: precise-object-edit
Asset type: revised production prop design reference sheet
Input image: edit target and approved base. Preserve the halo design exactly: one complete closed circular flat cable-tie-like metal band, thin rectangular cross-section, white/silver borders, graphite rear surface, orange-yellow front-face luminous inlay over about 80% of the circumference, the upper-right white mechanical lock housing, its diagonal fin, four-view layout, white background, proportions, and materials.
Primary edit: add a single rough dangling wire and one barcode tag to the existing mechanical lock housing. Change nothing else.
Wire: attach exactly one dark charcoal braided wire to a small socket on the rear/lower side of the upper-right mechanical housing. It should resemble the rough loose wire in the user's earlier sketch: hand-made, slightly uneven and kinked, with a loose downward-curving loop, coarse woven sheath, worn fuzzy fibers, small frayed spots, and tiny glimpses of metallic strands. It is an accessory tail, not part of the circular ring and not another halo arc. Keep it visibly separated from the clean circular band.
Tag: at the free end of the wire, attach one small rectangular off-white synthetic tag with clipped corners and a tiny metal eyelet. On its face place a simple black barcode made only of vertical bars of varied width. No digits, no letters, no readable text, no logo. The tag should be clearly visible in the front and rear views and enlarged alongside the wire texture in the detail panel.
Composition: retain four distinct views. Front and rear show the rough wire hanging outside the ring from the mechanical housing with the barcode tag at the end. Side view shows the separate attachment position. Detail panel focuses on the housing, flat band socket, braided wire fastener, frayed texture, and barcode tag.
Constraints: preserve the approved halo unchanged; exactly one wire; exactly one tag; barcode bars only; wire must look coarse, worn, braided, flexible, and physically attached to the housing; keep the wire and tag outside the ring opening as much as possible so they do not obscure the silhouette.
Avoid: redesigning the halo, changing the 80:20 ratio, opening the circle, adding more rings, smooth plastic cable, glowing wire, chain, rope tassel, multiple wires, multiple tags, QR code, numbers, letters, words, labels, logo, watermark, character, head, hands, scenery.
```

### 6차 검수
- 통과: 승인 베이스의 완전한 단일 원형 밴드와 80:20 구성이 유지됨.
- 통과: 허브에 연결된 거친 꼬임 와이어가 1가닥만 존재함.
- 통과: 와이어 끝에 바코드 태그가 1개만 존재함.
- 통과: 바코드는 검은 세로 막대로만 표현되고 읽을 수 있는 문자와 숫자가 없음.
- 통과: 상세 뷰에서 와이어 체결부와 닳고 보풀진 질감이 명확함.

## 7차 수정
- 사용자 정정: 거친 와이어는 허브와 착용자의 뒤통수 접속 패드를 연결하는 기능성 연결선.
- 바코드 태그는 와이어에서 분리하고 링 밴드의 좌측 하단에 작은 고리로 직접 결속.
- 결과: `07.png`

### 최종 프롬프트 (7차)

```text
Use case: precise-object-edit
Asset type: corrected production prop design reference sheet
Input image: edit target. Preserve the approved closed flat cable-tie halo, 80% orange luminous face inlay, 20% white upper-right mechanical housing, graphite backside, diagonal fin, overall proportions, materials, and white-background reference-sheet quality.
Correction: the rough wire and barcode tag currently hang together from the outside of the housing. REMOVE that incorrect arrangement completely and separate their functions as follows.
1. OCCIPITAL WIRE: exactly one short rough braided charcoal wire exits from the INNER face of the upper-right mechanical housing and travels inward toward the center of the halo, where it terminates in a low-profile round occipital contact pad that attaches to the back of the wearer’s head. The wire is an attachment tether between the halo housing and the back of the head. It must not hang downward outside the ring and must not carry the barcode tag. Preserve its coarse worn woven sheath, uneven bends, frayed fibers, and occasional exposed metallic strands.
2. BARCODE TAG: exactly one small off-white rectangular barcode tag is tied DIRECTLY AROUND THE FLAT HALO BAND at the lower-left section of the circle using a tiny separate black tie loop. The barcode tag is not attached to the rough occipital wire and not attached to the mechanical housing. It hangs a short distance from the lower-left band. Its face has only black vertical barcode bars of varying width, with no letters, numbers, or logo.
Composition: retain four panels but adapt them to communicate function. Front view shows the closed halo, the inward-pointing short wire and contact pad, and the separate tag tied at lower-left. Side attachment view may include only a very simple smooth matte-gray faceless mannequin head silhouette as a scale/fit proxy, showing the contact pad seated on the back of the head and the halo floating behind it; no hair or clothing. Rear view shows the wire path from housing to occipital pad and the separately tied tag. Detail panel shows both distinct attachments: rough wire entering the head contact pad, and a separate small loop fastening the barcode tag around the flat band.
Hard constraints: rough wire connects housing to back-of-head contact pad; barcode tag tied directly to the flat ring band; these are separate systems; exactly one wire, one contact pad, one tag; retain fully closed ring and 80:20 design; barcode bars only.
Avoid: tag attached to wire, tag attached to housing, wire hanging outside or downward, decorative tassel, wire loop around ring, multiple wires, multiple tags, readable text, numbers, QR code, redesigning the halo, opening the ring, extra rings, full character, face details, hair, clothing, scenery, watermark.
```

### 7차 검수
- 통과: 거친 와이어가 허브 안쪽에서 뒤통수 접속 패드로 이어짐.
- 통과: 착용 구조 뷰에서 접속 패드가 마네킹 뒤통수에 닿는 방식이 명확함.
- 통과: 바코드 태그가 와이어와 분리되어 링 밴드 좌측 하단에 직접 묶임.
- 통과: 단일 폐쇄형 금속 밴드와 80:20 디자인이 유지됨.

## 8차 수정
- 접속선을 짧은 1가닥에서 길게 늘어지는 거친 와이어 3가닥으로 변경.
- 세 와이어는 허브 안쪽의 개별 소켓과 공용 뒤통수 접속 패드를 연결하며 서로 다른 U자 곡선으로 처짐.
- 최초 결과 `08.png`에서는 바코드 태그가 링 밴드에 남아 있어 후속 수정.

## 9차 수정
- 사용자 추가 정정: 바코드 태그를 링 밴드에서 제거하고 우측 상단 안테나에 결속.
- 결과: `09.png`

### 최종 프롬프트 (9차)

```text
Use case: precise-object-edit
Asset type: corrected production prop design reference sheet
Input image: edit target. Preserve everything: the complete flat cable-tie halo, 80% orange luminous inlay, upper-right white mechanical housing, EXACTLY THREE long separate rough wires sagging in large loops between the inner housing and the shared occipital pad, mannequin fit view, materials, proportions, and layout.
Only correction: MOVE the single barcode tag from the lower-left halo band to the upper-right diagonal antenna. Remove the tag and its black loop completely from the lower-left ring band. Attach exactly one small off-white barcode tag to the upper portion of the diagonal antenna using a small separate black tie loop wrapped around the antenna. The tag hangs naturally beside the antenna, clear of the three rough occipital wires.
Barcode appearance: black vertical bars of varying widths only. No letters, digits, words, logo, QR code, or readable text.
Composition: front and rear views must show the tag tied to the antenna and no tag anywhere on the ring band. Side mannequin view should show the antenna tag separately from the long wires. Detail panel should show the antenna, black tie loop, and tag attachment while still preserving the three wire sockets.
Hard constraints: exactly one tag; tag on antenna only; zero tags on ring band; zero tags on the three wires; keep exactly three long sagging occipital wires; change nothing else.
Avoid: tag on band, tag on wire, multiple tags, short wires, merged cable bundle, readable text, redesigning halo, opening ring, extra rings, character details, scenery, watermark.
```

### 9차 검수
- 통과: 긴 거친 와이어가 3가닥으로 분리되어 허브와 뒤통수 패드를 연결함.
- 통과: 세 와이어가 짧거나 팽팽하지 않고 서로 다른 깊이의 U자 곡선으로 길게 처짐.
- 통과: 바코드 태그가 링과 와이어에서 제거되고 안테나에만 묶임.
- 통과: 단일 폐쇄형 금속 밴드, 80:20 비율, 색상과 재질이 유지됨.

## 10차 수정
- 기계장치 영역을 원 둘레 약 20%에서 약 12%로 축소하고 발광 밴드를 약 88%로 확대.
- 안테나 길이를 이전 대비 약 1.7배로 연장.
- 바코드 태그를 안테나 끝에서 뿌리 체결부로 이동.
- 접속선을 굵고 거친 검정 와이어 1가닥, 얇은 빨강 전선 1가닥, 얇은 파랑 전선 1가닥으로 변경.
- 결과: `10.png`

### 최종 프롬프트 (10차)

```text
Use case: precise-object-edit
Asset type: revised production prop design reference sheet
Input image: edit target. Preserve the approved complete flat cable-tie halo, white/silver metal borders, graphite rear face, warm orange front-face inlay, vertical placement behind the head, mannequin fit view, white background, and overall art quality.
Make these exact structural revisions:
1. SHRINK THE MECHANICAL HOUSING: reduce the upper-right white/graphite mechanical arc from about 20% to only about 12% of the ring circumference. Make it visibly more compact and less bulky while keeping recognizable angular white/silver armor and dark graphite internals. Extend the orange luminous band so it occupies about 88% of the circle. Preserve one perfectly closed ring.
2. LONGER ANTENNA: extend the single diagonal antenna to about 1.7 times its current length. Keep it slender, straight, white/graphite, and orange-lit.
3. TAG LOCATION: keep exactly one off-white barcode tag, but tie it at the ROOT of the antenna, immediately where the antenna emerges from the mechanical housing, using one small black loop. It must not sit near the antenna tip, the circular band, or any connection wire. Barcode contains black vertical bars only, no letters or digits.
4. CONNECTION LINES: replace the three equally thick black braided wires with exactly three long separate connection lines between distinct inner-housing sockets and distinct sockets on the shared occipital pad: ONE thick rough black braided cable, ONE much thinner smooth insulated red wire, and ONE much thinner smooth insulated blue wire. The red and blue wires are clearly separate solid colors and roughly one-quarter the diameter of the black cable. All three are longer than the direct distance and hang in large loose U-shaped loops with slightly different depths before rising to the occipital pad. The thick black cable retains worn braid, fuzz, fraying, and occasional exposed metal; red and blue wires are smoother but slightly scuffed.
Composition: retain a multi-view white-background reference sheet. Front view clearly shows the smaller 12% housing, longer antenna with tag at its root, and three color/diameter-distinct sagging lines. Side mannequin view clearly shows all three connecting to the back-of-head pad. Rear view preserves the graphite band and separate sockets. Detail views show the three wire types and the barcode tag at the antenna root.
Hard constraints: exactly one thick black cable; exactly one thin red wire; exactly one thin blue wire; exactly one tag at antenna root; antenna visibly longer; mechanical housing visibly smaller; closed circle; about 88% luminous band and 12% machinery.
Avoid: three black ropes, bundled or merged wires, short taut wires, extra wires, tag at antenna tip, tag on ring, tag on wire, oversized housing, opening the circle, extra rings, readable text, QR code, hair, clothing, scenery, watermark.
```

### 10차 검수
- 통과: 기계장치가 원 둘레 약 12%의 소형 허브로 축소됨.
- 통과: 안테나가 길어지고 태그가 안테나 뿌리에 묶임.
- 통과: 굵고 거친 검정 와이어 1가닥과 얇은 빨강·파랑 전선이 명확히 구분됨.
- 통과: 세 접속선 모두 길게 처져 뒤통수 패드에 연결됨.
- 통과: 단일 폐쇄형 밴드와 백색·흑연색·주황색 재질 구성이 유지됨.

## 11차 수정
- 바코드 태그의 가로·세로 크기를 각각 2배로 확대.
- 태그를 흠집과 오염이 없는 유광 백색 신제품 재질로 변경.
- 좌측 상단과 하단의 넓은 호 2구간을 금속 테두리 없는 전폭·전두께 발광 밴드로 변경.
- 나머지 링 구간은 금속 테두리와 매입형 발광 인레이 구조 유지.
- 결과: `11.png`

### 최종 프롬프트 (11차)

```text
Use case: precise-object-edit
Asset type: revised production prop design reference sheet
Input image: edit target. Preserve the approved complete flat cable-tie halo, compact 12% upper-right mechanical housing, long antenna, tag at antenna root, exactly one thick rough black cable plus one thin red wire and one thin blue wire connecting to the occipital pad, mannequin fit view, white background, proportions, and multi-view layout.
Make only these two design changes:
1. BARCODE TAG: make the single barcode tag exactly twice its current width and height, while retaining the same rectangular proportions and attachment at the ROOT of the antenna. Make it look pristine and newly manufactured: glossy smooth white polymer, crisp beveled edges, strong clean specular highlights, spotless surface, no scratches, no grime, no yellowing, no chipped corners. Barcode consists only of perfectly sharp black vertical bars; no letters, numbers, logo, or QR code. Keep one small clean black attachment loop at the antenna root.
2. FULLY LUMINOUS ARC SECTIONS: preserve the thin flat rectangular cable-tie cross-section and the closed circular silhouette. Most of the ring keeps its existing physical white/silver metal edges with a recessed orange luminous inlay. However, convert exactly TWO broad arc sections—one on the upper-left quadrant and one spanning the bottom quadrant—into fully luminous solid sections where the ENTIRE band width and full thickness glow warm golden-yellow to orange. In these two sections there are no visible metal borders on the front, sides, or edges: the full flat strap becomes a translucent solid light material. These must remain flat ribbon-like arcs with rectangular cross-section, not round tubes, beams, pipes, or neon hoses. Use clean mechanical transition collars at both ends of each fully luminous section so the change from metal-edged inlay band to all-light band is clearly readable.
Composition: in the front view, the upper-left and bottom full-width luminous arcs must be obvious and separated by normal metal-edged inlay sections. Rear view should show those same two full-light sections consistently. Detail panels should include one transition collar between the standard metal-edged band and fully luminous flat band, plus the enlarged glossy new tag at the antenna root.
Hard constraints: exactly one tag at antenna root, tag 2x size, pristine glossy new surface; exactly two full-width luminous arc sections; flat rectangular band cross-section throughout; one closed ring; preserve three connection lines and small housing.
Avoid: worn or dirty tag, tag at antenna tip, tag on ring, more than one tag, entire ring becoming pure light, round laser tube, neon tube, circular rod, opening ring, changing wires, enlarging housing, readable text, watermark.
```

### 11차 검수
- 통과: 바코드 태그가 이전보다 약 2배 크며 유광 백색 신제품 표면으로 표현됨.
- 통과: 태그 위치가 안테나 뿌리에 유지됨.
- 통과: 좌측 상단과 하단의 호 2구간은 금속 테두리 없이 밴드 전체가 발광함.
- 통과: 완전 발광 구간도 납작한 밴드 형상을 유지하며 원통형 레이저로 변하지 않음.
- 통과: 소형 허브와 검정·빨강·파랑 접속선 구성이 유지됨.

## 12차 수정
- 바코드 태그의 결속 위치를 안테나 중간에서 허브와 맞닿는 안테나 최하단 시작점의 베이스 칼라로 이동.
- 나머지 형태, 재질, 발광 구간과 접속선은 유지.
- 결과: `12.png`

### 최종 프롬프트 (12차)

```text
Use case: precise-object-edit
Asset type: corrected production prop design reference sheet
Input image: edit target. Preserve EVERYTHING except the exact attachment height of the barcode tag: the complete flat ring, two full-width luminous arc sections, standard inset-light sections, compact mechanical housing, long antenna, large glossy pristine white barcode tag, one thick rough black cable, thin red and blue wires, occipital pad, mannequin view, multi-view layout, colors, proportions, and white background.
Only edit: move the single barcode tag's black tie loop all the way DOWN to the absolute STARTING POINT of the antenna. The loop must wrap around the lowest antenna base collar exactly where the long antenna emerges from and touches the mechanical housing. It must sit immediately above the housing surface with no visible length of antenna between the housing and the tie loop. The tag hangs from that base collar beside the housing.
The tag must NOT be attached halfway up the antenna and must NOT be near the tip. In every front, side, rear, and detail view, show the same base attachment. Use the detail panel to clearly show the black loop encircling the antenna's bottommost root collar at the housing junction.
Preserve tag properties: twice-size large tag, glossy spotless new white polymer, sharp beveled edges, crisp black vertical barcode bars only, no digits or letters.
Hard constraints: one tag only; tag loop at absolute bottom of antenna root; zero gap between loop and housing junction; change nothing else.
Avoid: loop at mid-shaft, loop near tip, tag on ring, tag on wires, smaller tag, worn tag, redesigning any other component, readable text, watermark.
```

### 12차 검수
- 통과: 태그 결속 고리가 허브와 맞닿은 안테나 최하단 베이스 칼라에 위치함.
- 통과: 안테나 중간이나 끝에 별도 태그가 없음.
- 통과: 확대된 유광 태그, 완전 발광 호 2구간, 세 접속선 구성이 유지됨.

## 13차 수정
- 태그 고리를 안테나 최하단과 허브 사이에 틈 없이 조여, 태그 몸체가 공간 부족으로 위·바깥쪽으로 들리도록 변경.
- 완전 발광 호 2구간의 네 시작·끝 경계를 서로 다른 각도의 불규칙한 사선 및 쐐기형 접합으로 변경.
- 규칙적인 수직 절단과 원형 칼라 제거.
- 결과: `13.png`

### 최종 프롬프트 (13차)

```text
Use case: precise-object-edit
Asset type: revised production prop design reference sheet
Input image: edit target. Preserve the complete flat halo, two full-width luminous arc sections, compact housing, long antenna, large glossy white barcode tag, thick black cable, thin red and blue wires, occipital pad, mannequin view, colors, proportions, and multi-view layout.
Make these two exact corrections:
1. TAG JAMMED AT ANTENNA START: cinch the tag's small black tie loop around the absolute lowest antenna base collar with ZERO clearance between the loop and the mechanical housing. The loop is wedged tightly in the narrow junction where the antenna first emerges from the housing; there is literally no free antenna shaft below it and no empty space for the tag to hang downward. Because the tag is large and physically collides with the nearby housing armor, the tag body is forced to kick upward and outward at a rigid 35–45 degree angle, visibly propped up by the housing. It should look crowded, compressed, and sprung upward, while still pristine and glossy. Do not let it hang vertically.
2. IRREGULAR DIAGONAL LIGHT-ARC BOUNDARIES: remove the regular perpendicular black ring collars at all four ends of the two fully luminous arc sections. Each transition between the fully luminous flat band and the standard metal-edged inset-light band must be a different asymmetrical diagonal cut across the band width. Use four distinct slanted angles, roughly 25°, 40°, 55°, and 70° relative to the band edge, with slight uneven stepped or wedge-shaped profiles. The cuts should look designed but irregular, never parallel to each other, never perpendicular to the arc, and never like uniform circular collars. Mark each transition only with a thin dark graphite oblique seam following the diagonal cut. Preserve the closed flat rectangular band.
Composition: front and rear views must clearly show all four nonmatching diagonal transition seams. Detail view should focus on the jammed antenna-root tag and at least one irregular diagonal luminous transition.
Hard constraints: tag loop touching housing with zero gap; tag visibly forced upward/outward; no vertical dangling tag; exactly two full-width luminous arcs; four irregular diagonal endpoints; no regular collars; preserve all other components.
Avoid: tag at mid-shaft or tip, tag hanging down, loose loop, perpendicular transition lines, circular ring collars, symmetrical matching cuts, round neon tube, opened ring, changed wires, readable text, watermark.
```

### 13차 검수
- 통과: 태그 고리가 허브와 안테나 시작점 사이에 틈 없이 밀착됨.
- 통과: 큰 태그가 아래로 늘어지지 않고 위·바깥쪽으로 들려 있음.
- 통과: 완전 발광 호의 네 경계가 서로 다른 사선·쐐기 형태임.
- 통과: 규칙적인 수직 경계와 원형 칼라가 제거됨.
- 통과: 폐쇄형 링, 소형 허브, 검정·빨강·파랑 접속선이 유지됨.
