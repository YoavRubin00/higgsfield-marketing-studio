# Higgsfield Marketing Studio — מסמך הקשר ראשי

מסמך זה נטען בכל סשן Claude Code בתיקייה הזו. הוא מתעדכן עם הזמן.

---

## מי המשתמש

**יואב רובין** (yrubin00@gmail.com). בונה מותג עצמאי משלו עם פוקוס ב**תוכן לרשתות חברתיות + פרסומות וידאו / UGC** באמצעות Higgsfield AI.

## על המותג

> **TODO**: למלא לאחר שיחה עם המשתמש על המותג.
> ראה [BRAND/brand-kit.md](BRAND/brand-kit.md) למילוי מסודר.

- שם המותג: _____
- נישה: _____
- ICP (קהל יעד): _____
- מסר מרכזי: _____
- פלטפורמות עיקריות: _____

---

## חוקי ברירת מחדל

### שפה
- **עברית בלבד** לכל פלט הפונה לקהל: קופי, קריינות, captions, hashtags, alt text.
- **שמות קבצים באנגלית** (מערכת קבצים).
- מסמכי עבודה פנימיים — עברית, אבל מקסם clarity.

### ארגון פלטים
- כל פלט סופי הולך ל-`CONTENT/<YYYY-MM>/<YYYY-MM-DD>_<topic>/`
  - `brief.md` — מה רצינו לעשות
  - `script.md` — קופי + סקריפט קריינות
  - `prompts.md` — פרומפטים שהשתמשו ב-Higgsfield/ElevenLabs
  - `outputs/` — התוצרים (mp4, png, mp3)
  - `publish.md` — הקופי הסופי לפרסום + hashtags
- **נכסים גולמיים** (לא תוצרים סופיים) ל-`ASSETS/`.
- **מחקרים** ל-`RESEARCH/<YYYY-MM-DD>_<topic>/`.

---

## ניתוב סקילים — מה להשתמש מתי

| משימה | סקיל מומלץ |
|---|---|
| מחקר עומק על נושא/קהל/מתחרה (עברית) | `חוקר` |
| טרנדים מ-30 ימים אחרונים | `last30days` |
| תובנות מ-Reddit על נישה | `reddit-insights` |
| ניתוח מתחרים מתוך URLs | `competitor-profiling` |
| רעיונות לתוכן מבוססי positioning | `content-idea-generator` |
| תכנון אסטרטגיית תוכן | `content-strategy` |
| כתיבת קופי לפוסט/ריל | `social-content` או `copywriting` |
| לוודא איכות ציוץ/פוסט קצר | `tweet-draft-reviewer` |
| לחלץ AI-jargon מקופי | `de-ai-ify` |
| חילוץ קול מותג מדגימות | `voice-extractor` |
| תמונת מוצר מקצועית | `higgsfield-product-photoshoot` |
| תמונה / וידאו כללי + Marketing Studio | `higgsfield-generate` |
| אימון Soul ID (דמות עקבית) | `higgsfield-soul-id` |
| כרטיסי מוצר ל-marketplace | `higgsfield-marketplace-cards` |
| מיצוב מותג | `positioning-basics` |
| psychological frameworks לקופי | `marketing-psychology` |

---

## Higgsfield Stack — קונפיג של ultimate plan

### מודלים שצריך להכיר
- **Soul V2** — דמות עקבית (אחרי `higgsfield-soul-id`). הכי טוב ל-talking head.
- **Seedance 2.0** — UGC עם lip-sync טבעי, ספיש + תמונה במעבר אחד.
- **Kling 3.0** — motion control, frame-by-frame. ל-action sequences.
- **Veo 3.1** — קולנועי, איכות גבוהה. ליריות יוקרתיות.
- **Sora 2** — וידאו 12 שניות 1080p, ריאליסטי.
- **Cinema Studio 3.5** — שימוש בנוסחת MCSLA לסצנות מובנות.
- **Nano Banana 2** — תמונות 4K זריזות.
- **GPT Image 2** — טקסט בתמונה (חשוב למוטיב עם כיתובים).
- **Flux 2** — יצירה מבוססת reasoning.

### גבולות ידועים
- **וידאו: 12-15 שניות מקסימום** — לתוכן ארוך יותר, צריך לרכב כמה שוטים.
- **אין פרסום native לרשתות** — צריך ידני / Playwright / Buffer.
- **קרדיטים: 0** ⚠️ — לפני generation, **לטעון קרדיטים**.
- **אין editing native** — לרכבת וידאו צריך CapCut/Descript.

### Marketing Studio modes
- **UGC**: talking heads, product reviews, unboxings, virtual try-ons
- **Professional**: CGI showcases, cinematic demos
- **Narrative**: TV spot מלאים, branded storytelling
- **Wild Card**: ה-AI מנהל את כל הכיוון הקריאטיבי

### Product Photoshoot — 10 modes
`product_shot`, `lifestyle_scene`, `closeup_product_with_person`, `moodboard_pin`, `hero_banner`, `social_carousel`, `ad_creative_pack`, `virtual_model_tryout`, `conceptual_product`, `restyle`.

---

## Workflows מוכנים (בתיקיית TEMPLATES/)

1. **Reactive Content** — מטרנד לפוסט תוך 15-20 דק'
2. **UGC Ad Pipeline** — מ-brief לוידאו ad מוכן עם קריינות + מוזיקה
3. **Soul-Led Series** — סדרת תכנים עם דמות עקבית
4. **Content Calendar 30 יום** — תכנון חודשי
5. **Brand Voice Capture** — חילוץ קול מותג מדגימות

ראה תבניות ספציפיות ב-[TEMPLATES/](TEMPLATES/).

---

## MCPs פעילים בפרויקט

| MCP | מצב | שימוש |
|---|---|---|
| Higgsfield | ✅ | יצירת תמונות/וידאו, Soul ID, Marketing Studio |
| Neon | ✅ | DB אם נצטרך |
| Google Drive | ✅ | סינכרון נכסים |
| ElevenLabs | TBD | TTS עברית — להתקין Phase 1 |
| Playwright | TBD | אוטומציה לדפדפן — להתקין Phase 1 |
| Notion | TBD | content calendar — להתקין Phase 1 |
| Suno | TBD | מוזיקה — להתקין Phase 2 |

---

## תזכורות שוטפות

- **לבדוק קרדיטי Higgsfield** לפני generation: `mcp__higgsfield__balance`
- **לעדכן `BRAND/prompt-library.md`** עם פרומפטים שעובדים — כל פעם שמשהו יוצא טוב.
- **לעדכן `BRAND/soul-ids.md`** אחרי כל אימון Soul חדש (reference_id + תמונת preview).
- **memory file** ב-`memory/MEMORY.md` — לעדכן עם תובנות גדולות על המותג.

---

## הקשר טכני (Windows + Hebrew path)

- הנתיב הביתי מכיל עברית (`יואב רובין`) — חבילות npm עם tar postinstall יכולות להיכשל. חלופה: הורד בינארי ל-`C:\Tools\<name>\` והוסף ל-PATH.
- Higgsfield CLI: `C:\Tools\higgsfield\hf.exe` (כבר ב-PATH).

ראה [memory/environment_hebrew_path.md](C:/Users/יואב רובין/.claude/projects/c--Users-------------claude-projects-higgsfield-marketing-studio/memory/environment_hebrew_path.md) לפרטים.
