# CICAN CIA

An independent learning and discovery interface for the publicly available CIA FOIA Electronic Reading Room.

## Experience

**DISCOVER → DECODE → READ**

The CIA Reading Room remains the authoritative primary source. CICAN CIA is the accessibility layer.

## Game foundation

The decode interaction preserves the established CICAN language:
- Start size: 34
- Growth: +0.5
- Maximum size: 180
- Movement interpolation: x += (targetX - x) * 0.10; y += (targetY - y) * 0.10
- Double-tap split: 350 ms
- Split placement: 45 px
- Merge distance: 20 px
- FULL + FULL → READ unlock
- FULL + small and small + small can merge without unlocking READ

No CIA record is fabricated. The next stage is the real source/search layer connecting topics to exact CIA Reading Room records.

Official source: https://www.cia.gov/readingroom/
