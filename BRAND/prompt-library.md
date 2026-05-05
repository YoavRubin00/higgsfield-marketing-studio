# Prompt Library — FinPlay

> אוסף פרומפטים שעובדים — ויזואל, קריינות, קופי. כל פעם שמשהו יוצא טוב — להוסיף כאן.

---

## ElevenLabs — קריינות עברית

### הקול הראשי של המותג: **Liam**

```
Voice ID: TX3LPaxmHKxFdv7V0QHJ
Model:    eleven_v3
```

זה הקול שמשמש בסקריפטים של האפליקציה ([finpl/scripts/generate_module_audio.js](C:/Users/יואב רובין/.claude/projects/finpl/scripts/generate_module_audio.js)). שומר על עומק, סמכות, ואופי דיבור עקבי על פני כל המודולים.

### הגדרות מומלצות (התחלה)
- **stability**: 0.5 (ניטרלי) או 0.65 (עקבי יותר לקריינות מודולית)
- **similarity_boost**: 0.75
- **style**: 0.3-0.4 (טון מבוקר; גבוה מדי = דרמטי מדי)
- **use_speaker_boost**: true

### דוגמת קריאה ב-MCP

```
mcp__ElevenLabs__text_to_speech(
  text: "...",
  voice_id: "TX3LPaxmHKxFdv7V0QHJ",
  model_id: "eleven_v3",
  stability: 0.65,
  similarity_boost: 0.75,
  style: 0.35
)
```

### Tips לכתיבת סקריפט עברית
- **מספרים במילים**: "שלוש" במקום "3" (ב-eleven_v3 משופר אבל עדיין יציב יותר ככה)
- **פסיקים ופוינטים** = הפסקות. השתמש בקפידה.
- **אנגליציזמים** (Apple, Excel, TikTok) — ההגייה לא תמיד מושלמת. שקול לכתוב פונטית או להחליף בעברית.
- **דגימה קצרה לפני שיוצרים סקריפט מלא** — לבדוק שההגייה מקובלת.

### דוגמאות סגנון לקריינות לפי תוכן
- **למידה רגילה (מודול)**: stability 0.65, style 0.35 — מאוזן, סמכותי-נעים
- **Hook ברגש (פתיח של ריל)**: stability 0.4, style 0.6 — יותר אנרגטי
- **כתוביות סיכום (אאוטרו)**: stability 0.7, style 0.25 — רגוע, מסכם

---

## Higgsfield — תמונות לאפליקציה (Nano Banana / GPT Image)

### Style guide גלובלי לתמונות מודולים

```
A minimalist, flat vector illustration representing [CONCEPT]. 
Keep it completely text-free. 
Deep blue and cyan palette, clean geometry, negative space, 
premium fintech aesthetic, highly polished.
```

**5 רכיבים שאסור להחסיר**:
1. `minimalist, flat vector illustration` — לא 3D, לא ציור שמן
2. `completely text-free` או `no text whatsoever` — AI הוזה טקסט בעברית
3. `Deep blue and cyan palette` — קונסיסטנטיות מותג בכל המודולים
4. `clean geometry, negative space` — אסתטיקת fintech מודרנית
5. `premium fintech aesthetic` — לא clip-art

מקור מלא: [finpl/INFOGRAPHIC_RECIPE.md](C:/Users/יואב רובין/.claude/projects/finpl/INFOGRAPHIC_RECIPE.md)

---

## Higgsfield — תמונות לתוכן חברתי (פוסטים, ריילים)

### Style 1: Brand Educational (רגיל, חינוכי)
```
A minimalist flat vector illustration representing [CONCEPT].
Deep blue and cyan palette, clean geometry, negative space,
premium fintech aesthetic. Vertical 9:16 composition.
NO TEXT, NO LETTERS.
```

### Style 2: UGC Authentic (חי, גולמי)
```
Real-life photo of person using mobile finance app at [LOCATION:
coffee shop / office desk / bedroom evening]. Natural light,
casual outfit, slight motion blur, authentic Instagram aesthetic.
9:16 vertical.
```

### Style 3: Bullshit Swipe (לפרסומות שמלגלגות על הז'אנר)
לסגנונות "spam aesthetic" שלפעמים שימושיים לסטוריטלינג של "ככה זה נראה כשמנסים לרמות אותך":

ראה [finpl/NANO-BANANA-PROMPTS.md](C:/Users/יואב רובין/.claude/projects/finpl/NANO-BANANA-PROMPTS.md) — יש שם 12 templates של:
- Scam neon (ורוד-סגול ניאון)
- Crypto scam (כחול כהה + זהב)
- MLM aspirational (פסטל פייטה)
- Tech conspiracy (matrix dark)
- Real estate scam (בלו-אאוואר + מטבעות)

---

## Higgsfield — וידאו (Cinema Studio MCSLA)

ראה [TEMPLATES/mcsla-recipes.md](../TEMPLATES/mcsla-recipes.md) למתכונים.

### דוגמה — Talking head מציג טיפ פיננסי
```
M: soul_cinema_studio (אם יש Soul ID)
   או seedance_2_0 (avatar מהגלריה)
C: medium close-up, subtle push-in 4%, eye-level
S: presenter casual ב-30+, smartwatch ביד, חולצת cotton פשוטה
L: תאורת window key + soft fill, צבעים נטרליים, מרגיש
   "מקצועי אבל לא מסחרי"
A: מסתכל למצלמה, מדבר טבעי, מחוות יד מינימליות,
   חיוך קל בסוף
Voiceover: <עברית סקריפט 8-12 שניות, Liam voice>
Duration: 10s
```

### דוגמה — App showcase (UI on mobile)
```
M: kling_3_0
C: locked top-down, יד מחזיקה טלפון
S: יד צעירה, גוון עור טבעי, האפליקציה FinPlay על המסך
L: תאורת חלון רכה, שולחן עץ ברקע, קצת bokeh
A: גלילה אטית במסך, תקריב על XP counter שעולה,
   חיוך מתחת לפריים
Duration: 6s
```

---

## Marketing Studio — UGC modes לפי סוג תוכן

### Talking head — explainer
```
Avatar: <Soul ID של presenter קבוע>
Hook (3 שניות ראשונות): "[משפט hook חזק בעברית]"
Body: "[3-4 משפטים על הקונספט הפיננסי]"
CTA: "FinPlay בלינק בביו"
Mode: UGC > talking head
Voice: ElevenLabs Liam (TX3LPaxmHKxFdv7V0QHJ)
Length: 30s
```

### Demo / Walkthrough
```
Mode: UGC > tutorial
Show: smartphone screen recording של האפליקציה
Voiceover: ElevenLabs Liam מסביר מה רואים
Captions: עברית on-screen תמיד
Length: 30-45s
```

---

## Suno — מוזיקה (כשנוסיף)

### Style 1: Lo-fi chill (לרגעי לימוד באפליקציה / B-roll)
```
lo-fi hip hop, mellow, daytime, no vocals, 90 BPM
```

### Style 2: Upbeat learning (לפתיח/אאוטרו)
```
indie pop, energetic, optimistic, female vocals optional,
hook at second 3, 110-120 BPM
```

### Style 3: Tense gaming (לסצנות "החלטה גורלית" / Bullshit Swipe)
```
electronic synthwave, building tension, no vocals, 100 BPM,
sharp drop at second 8
```

---

## קופי — formulas שמתאימים ל-FinPlay

### Hook — Pattern 1: Question with bite
```
"אם בכל פעם שאתה רואה משכורת אתה חושב 'איך זה כבר הלך?' — תקרא את זה."
```

### Hook — Pattern 2: Confession
```
"שילמתי 10K לכלכלן והוא נתן לי טבלה שיכולתי להכין לבד ב-25 דקות."
```

### Hook — Pattern 3: Counter-intuitive
```
"להפסיק לחסוך זה הצעד הראשון לעשירות אמיתית. ובכן — לא בדיוק."
```

### Body — Pattern: Problem → Reframe → Action
```
[Problem] רוב האנשים חושבים שהבעיה היא הכנסה.
[Reframe] בפועל — הבעיה היא לא לדעת *לאן* הכסף הולך.
[Action] FinPlay מלמד אותך לראות. בלי שיחות פיננסים. במשחק.
```

---

## הערות והוראות

- **כל פעם שמייצר תוכן ל-FinPlay**, התחל בקריאת [BRAND/voice.md](voice.md) ו-[BRAND/brand-kit.md](brand-kit.md).
- **אם יוצא טוב — תוסיף לכאן** עם תיאור קצר של המקרה.
- **אם משהו לא עובד — תוסיף לתחתית בסקציית "מה לא עבד"** עם הסבר קצר.

---

## מה לא עבד (יומן)

> שמור פה כשלונות מנע. חוסך זמן בעתיד.

- _ריק לעת עתה._
