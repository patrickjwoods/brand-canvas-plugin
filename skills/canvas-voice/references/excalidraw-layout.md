# Excalidraw Layout Reference

When the canvas is complete, generate `brand-canvas.excalidraw` using this spec.

---

## Visual Structure

```
┌────────────────────────────────────────────────────────────────────────┐
│              BRAND STRATEGY CANVAS — [Company Name]                    │  y=0, h=60
├──────────────────┬────────────────────────────┬────────────────────────┤
│ A. Customer/User │ B. Competitive Environment  │ C. Features            │  y=60, h=200
│    Insight       │                             │                        │
├──────────────────┤                             ├────────────────────────┤
│ Rational         │ ┌─────────────────────────┐ │ Values                 │  y=260, h=200
│ Benefits         │ │                         │ │                        │
├──────────────────┤ │  POSITIONING STATEMENT  │ ├────────────────────────┤
│ Emotional        │ │                         │ │ Personality            │  y=460, h=200
│ Benefits         │ │  Brand Essence: ...     │ │                        │
├──────────────────┴─┴─────────────────────────┴─┴────────────────────────┤
│                          KEY MESSAGES                                   │  y=660, h=200
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Box Coordinates

| Box | x | y | w | h | Background |
|-----|---|---|---|---|------------|
| Title bar | 0 | 0 | 1560 | 60 | #1971c2 |
| A. Customer/User Insight | 0 | 60 | 420 | 200 | #e7f5ff |
| B. Competitive Environment | 420 | 60 | 720 | 200 | #e7f5ff |
| C. Company/Product Features | 1140 | 60 | 420 | 200 | #e7f5ff |
| Rational Benefits | 0 | 260 | 420 | 200 | #ebfbee |
| Positioning Statement | 420 | 260 | 720 | 400 | #fff9db |
| Values | 1140 | 260 | 420 | 200 | #f3f0ff |
| Emotional Benefits | 0 | 460 | 420 | 200 | #ebfbee |
| Personality | 1140 | 460 | 420 | 200 | #f3f0ff |
| Key Messages | 0 | 660 | 1560 | 200 | #f3f0ff |

---

## Color Scheme

- **Title bar**: background `#1971c2`, text `#ffffff`
- **Market Opportunity** (A, B, C): `#e7f5ff` (light blue)
- **Benefits** (Rational, Emotional): `#ebfbee` (light green)
- **Positioning Statement**: `#fff9db` (warm cream) — the center of the canvas
- **Voice** (Values, Personality, Key Messages): `#f3f0ff` (light purple)
- **Box stroke**: `#1e1e1e` on all boxes
- **Body text**: `#1e1e1e`

---

## Element Structure

Each box requires 3 elements in `elements[]`:
1. A **rectangle** (the colored box)
2. A **title text** (section label, `fontSize: 13`, all-caps, `x+10, y+8`)
3. A **body text** (content, `fontSize: 11`, `x+10, y+30`, `width-20`)

**Rectangle element:**
```json
{
  "id": "rect_A",
  "type": "rectangle",
  "x": 0, "y": 60, "width": 420, "height": 200,
  "angle": 0,
  "strokeColor": "#1e1e1e",
  "backgroundColor": "#e7f5ff",
  "fillStyle": "solid",
  "strokeWidth": 2,
  "strokeStyle": "solid",
  "roughness": 0,
  "opacity": 100,
  "groupIds": [], "frameId": null, "roundness": null,
  "seed": 1003, "version": 1, "versionNonce": 1003,
  "isDeleted": false, "boundElements": null,
  "updated": 1700000000000, "link": null, "locked": false
}
```

**Text element (add these fields on top of the rectangle fields):**
```json
{
  "type": "text",
  "backgroundColor": "transparent",
  "strokeWidth": 1,
  "text": "A. CUSTOMER/USER INSIGHT",
  "fontSize": 13,
  "fontFamily": 2,
  "textAlign": "left",
  "verticalAlign": "top",
  "containerId": null,
  "originalText": "A. CUSTOMER/USER INSIGHT",
  "lineHeight": 1.25,
  "autoResize": false
}
```

Use sequential integers for `seed` / `versionNonce` (1001, 1002, 1003…). Use `1700000000000` for all `updated` values.

---

## Content Truncation

Each box is fixed-size — truncate content to fit. Add `...` if truncated.

| Box | Max chars |
|-----|-----------|
| A. Customer/User Insight | 300 |
| B. Competitive Environment | 400 |
| C. Company/Product Features | 300 |
| Rational Benefits | 260 |
| Emotional Benefits | 260 |
| Positioning Statement | full statement + brand essence (no truncation) |
| Values | 260 |
| Personality | 260 |
| Key Messages | all 3 messages, no proof points (full-width row) |

For Positioning Statement body text: write the full statement, then a blank line, then `Brand Essence: [essence]`.

---

## Element Order in `elements[]`

Generate elements in this order (each box = rect, title text, body text):
1. Title bar rect + title text (seed 1001–1002)
2. Box A rect + title + body (seed 1003–1005)
3. Box B rect + title + body (seed 1006–1008)
4. Box C rect + title + body (seed 1009–1011)
5. Rational Benefits rect + title + body (seed 1012–1014)
6. Positioning Statement rect + title + body (seed 1015–1017)
7. Values rect + title + body (seed 1018–1020)
8. Emotional Benefits rect + title + body (seed 1021–1023)
9. Personality rect + title + body (seed 1024–1026)
10. Key Messages rect + title + body (seed 1027–1029)

---

## Root JSON Structure

```json
{
  "type": "excalidraw",
  "version": 2,
  "source": "brand-strategy-canvas",
  "elements": [ ...all 29 elements... ],
  "appState": {
    "gridSize": null,
    "viewBackgroundColor": "#ffffff"
  },
  "files": {}
}
```

---

## Title Bar Text

```json
{
  "id": "text_title",
  "type": "text",
  "x": 10, "y": 12,
  "width": 1540, "height": 36,
  "strokeColor": "#ffffff",
  "text": "BRAND STRATEGY CANVAS — [COMPANY NAME]",
  "fontSize": 22,
  "fontFamily": 2,
  "textAlign": "center",
  ...
}
```
