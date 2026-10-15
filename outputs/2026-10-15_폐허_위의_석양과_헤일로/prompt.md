# 폐허 위의 석양과 헤일로

## 사용 파일
- 캐릭터: `characters/청록_장발_소녀.md`
- 스타일: `styles/선명한_애니메이션_일러스트.md`
- 캐릭터 레퍼런스: `refs/Untitled.jpeg`
- 소품: `props/사이버펑크_헤일로.md`

## 생성 설정
- 생성 방식: built-in image generation
- 비율: 세로 2:3
- 결과: `01.png`

## 최종 프롬프트 원문

```text
Use case: illustration-story
Asset type: polished vertical character illustration
Input image: the provided local reference is the strict character appearance and outfit reference. Preserve her recognizable face, hair, colors, clothing, and proportions.

Style/medium: polished contemporary anime character illustration; clean expressive line art; crisp cel shading blended with soft painted gradients; luminous eyes; highly detailed flowing hair; cinematic environment painting; saturated accents with atmospheric depth.

Subject and fixed appearance: One young woman with a slender build and fair skin. Extremely long, voluminous teal hair reaching below the waist, dark navy-teal at the crown and bangs transitioning into bright turquoise, mint, and green toward the outer strands and tips. Multiple sweeping locks and the distinctive curled ahoge on top. Large bright teal eyes, delicate youthful face. She wears the exact reference outfit: cropped taupe-gray short-sleeved hooded jacket with dark hood and cords and orange piping; black choker; white crop top with the orange outlined triangular motif centered on the chest; dark navy frayed denim shorts; black belt with silver rectangular buckle; black strapped utility pouch on her right thigh; black wrist bands; dark plum high-top sneakers with white laces and soles.

Halo prop: Behind her head floats exactly one complete circular cyberpunk halo, about 45 cm outer diameter, oriented vertically. It is a thin flat rectangular white/silver metal strap, cable-tie-like rather than a tube. About 88% is warm yellow-to-orange luminous inlay and two broad fully glowing flat arc sections at upper-left and bottom; about 12% at upper-right is a compact angular white/silver mechanical locking hub with graphite internals and warm orange seams. One long tangent rod antenna extends leftward from the upper-right hub within the ring plane. At the antenna root, pressed tightly against the hub, a clean glossy white barcode tag angles upward/outward, with black barcode bars only and no readable characters. From the inner hub, one thick rough black wire and two thin red and blue wires hang in distinct loose U-curves to a single rear-head connection pad. Keep the halo behind the head so it does not cover her face.

Scene/backdrop: She stands on the broken upper edge of a collapsed high-rise at dusk, surrounded by cracked concrete slabs, exposed rebar, shattered beams, rubble, and fragments of a ruined city below. She is looking slightly downward toward the sunset-lit city and horizon below her, calm, reflective, and quietly resolute.

Composition/framing: vertical 2:3 portrait, three-quarter to nearly full-body hero composition. Camera is directly in front of her at approximately chest height. Her face is front-facing and clearly visible, both eyes readable, with only a slight downward tilt of the gaze. Hair and jacket hems move gently in the high-altitude breeze. Strong silhouette against the open ruined skyline. No other people.

Lighting/mood: warm orange-pink sunset light bathes the ruined city and rims her hair, contrasted with cool teal shadows. Soft frontal fill light preserves all facial features and teal eyes. The sun itself is completely outside the frame and must not appear as a disc, glow-ball, or partial orb anywhere.

Constraints: preserve the reference character identity and exact fixed appearance; exactly one halo ring; one character only; face unobstructed and front-facing; no visible sun; no religious symbols; no angel wings; no crown; no text, captions, logos, or watermark.
Avoid: side profile, back view, face hidden by hair or halo, silhouetted face, visible solar disc, extra rings, neon tube halo, blue or cyan halo glow, short hair, missing ahoge, outfit redesign, extra limbs, malformed hands, extra fingers, photorealism, 3D render, chibi.
```

## 네거티브
- side profile, back view, face hidden by hair or halo, silhouetted face
- visible solar disc, glow-ball, partial sun orb
- extra rings, neon tube halo, blue or cyan halo glow
- short hair, missing ahoge, outfit redesign
- extra characters, extra limbs, malformed hands, extra fingers
- religious symbols, angel wings, crown
- photorealism, 3D render, chibi
- text, captions, logos, watermark

## 검수 결과
- 통과: 짙은 남청록에서 민트·초록으로 이어지는 허리 아래 길이의 머리.
- 통과: 정수리의 둥글게 말린 아호게와 청록색 눈.
- 통과: 회갈색 짧은 후드 재킷, 주황색 파이핑, 흰 크롭 탑의 주황 삼각형.
- 통과: 해진 짙은 데님 쇼츠, 벨트, 허벅지 파우치, 자주색 하이톱.
- 통과: 얼굴이 정면으로 선명하게 보이며 두 눈을 확인할 수 있음.
- 통과: 폐허가 된 고층 건물의 상부와 아래쪽 파괴된 도시가 명확함.
- 통과: 따뜻한 석양광은 있으나 태양 원반은 화면에 나타나지 않음.
- 통과: 단일 원형 헤일로, 온색 발광, 우측 상단 기계 허브, 접선형 안테나, 바코드 태그와 연결선이 표현됨.
- 재시도: 없음. 1차 결과를 최종 선택.

## 수정본 02
- 결과: `02.png`
- 비율: 세로 2:3
- 변경 사항: 전신 구도에서 허벅지 위 중심의 극적인 로우앵글로 변경. 한 손을 눈썹 위에 수평으로 들어 차양을 만들고, 강한 눈부심으로 눈을 가늘게 뜨며 눈살을 찌푸린 표정으로 변경.
- 광원 수정: 태양 원반은 화면 밖에 유지. 밝은 석양 하늘이 인물 뒤를 채우던 구성을 제거하고, 배경 하늘과 폐허 도시는 깊은 남색·청회색 어둠으로 낮춤. 카메라 쪽 프레임 밖의 낮은 태양광이 손, 팔, 얼굴, 가슴과 복부 정면을 강하게 비추도록 설정.
- 명암 수정: 손 아래 눈가에 뚜렷한 투영 그림자를 만들고, 따뜻한 정면 직사광과 차가운 배경 암부의 키아로스쿠로 대비를 강화.
- 검수 통과: 로우앵글, 비전신 크롭, 손 차양, 찌푸린 표정, 정면 태양광, 어두운 배경 대비, 보이지 않는 태양 원반, 단일 헤일로와 캐릭터 고정 외형.
- 시도 내역: 첫 수정에서 지평선의 작은 태양 원반을 제거했으나 배경 역광 인상이 남아, 최종 시도에서 배경 노출과 광원 방향을 전면 재설계함.
