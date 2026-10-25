# 에셋 목록

원본 파일은 `Assets/` 폴더에 있다. MannequinsXR은 엔진 VR 템플릿에 포함돼 있어 레포에 넣지 않았다.

---

## 1. 블록 텍스처

**Minetest Game 기본 텍스처** — https://github.com/luanti-org/minetest_game/tree/master/mods/default/textures

| 파일 | 사용처 |
|---|---|
| `default_grass.png` | 풀 블록 윗면 |
| `vrm_grass_side.png` | 풀 블록 옆면 (`default_dirt.png`에 `default_grass_side.png`를 합성) |
| `default_dirt.png` | 흙 블록, 풀 블록 아랫면 |
| `default_stone.png` | 돌 블록 |
| `default_cobble.png` | 조약돌 블록 (돌을 부수면 획득) |
| `default_sand.png` | 모래 블록 |
| `default_gravel.png` | 자갈 블록 |
| `default_tree_top.png` | 통나무 윗면·아랫면 |
| `default_tree.png` | 통나무 옆면 |
| `default_wood.png` | 판자 블록 |
| `default_leaves.png` | 나뭇잎 블록 |
| `default_glass.png` | 유리 블록 |
| `default_obsidian.png` | 기반암 블록 (맵 바닥, 파괴 불가) |

---

## 2. 손

**MannequinsXR (Unreal Engine VR Template)** — https://dev.epicgames.com/documentation/en-us/unreal-engine/vr-template-in-unreal-engine

| 파일 | 사용처 |
|---|---|
| `SKM_MannyXR_left` / `SKM_MannyXR_right` | 왼손 / 오른손 메시 |
| `ABP_MannequinsXR` | 트리거·그립 입력에 따른 손가락 애니메이션 |

---

## 3. 효과음

**Impact Sounds (Kenney)** — https://kenney.nl/assets/impact-sounds

| 파일 | 사용처 |
|---|---|
| `impactMining_*` | 돌·조약돌 파괴 |
| `impactWood_medium_*` | 통나무·판자 파괴 |
| `impactSoft_medium_*` | 흙·풀·모래·자갈·나뭇잎 파괴 |
| `impactGlass_heavy_*` | 유리 파괴 |
| `impactGeneric_light_*` | 블록 설치 |
| `footstep_grass_*` | 풀·흙 위 발소리 |
| `footstep_concrete_*` | 돌 위 발소리 |
| `footstep_wood_*` | 나무 위 발소리 |

**Interface Sounds (Kenney)** — https://kenney.nl/assets/interface-sounds

| 파일 | 사용처 |
|---|---|
| `switch_*` | 핫바 슬롯 전환 |
| `error_*` | 설치 불가 (블록 개수 0, 플레이어와 겹침) |

**Music Jingles (Kenney)** — https://kenney.nl/assets/music-jingles

| 파일 | 사용처 |
|---|---|
| `8-Bit jingles/jingles_NES13` | 단계 클리어 |
| `8-Bit jingles/jingles_NES00` | 최종 클리어 |

---

## 4. 배경음

**Birds and Wind – Ambient** — https://opengameart.org/content/birds-and-wind-ambient-birds-wind-and-synth

| 파일 | 사용처 |
|---|---|
| `birds_and_wind_ambient.ogg` | 지상 배경음 |

**Wind Whoosh Loop** — https://opengameart.org/content/wind-whoosh-loop

| 파일 | 사용처 |
|---|---|
| `wind_whoosh_loop.ogg` | 높은 곳 바람 소리 (3단계 탑) |

---

## 5. 폰트

**Galmuri** — https://github.com/quiple/galmuri

| 파일 | 사용처 |
|---|---|
| `Galmuri11.ttf` | 손목 위젯의 블록 개수, 목표 진행도, 클리어 시간 |

---

## 6. 맵

맵은 외부 에셋 없이 `BP_VoxelWorld` 블루프린트가 엔진 기본 큐브(`/Engine/BasicShapes/Cube`)와 위 블록 텍스처로 직접 쌓는다.
