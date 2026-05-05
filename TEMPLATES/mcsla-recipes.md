# MCSLA Recipes — נוסחאות Cinema Studio

> **MCSLA** = Model · Camera · Subject · Look · Action
> נוסחה רשמית של Higgsfield ל-Cinema Studio. הופכת פרומפט חלש לפלט מקצועי.
> ככל שכל ה-5 ברורים — הפלט יציב יותר.

---

## הסבר ה-5 רכיבים

### M — Model

**ברירת המחדל**: `kling_3_0`. מודלים אחרים — רק באישור מפורש של המשתמש.

- `kling_3_0` ← *ברירת מחדל*. Motion control גבוה, frame-by-frame, עד 15 שניות.
- `soul_cinema_studio` — מותר אם יש Soul ID של presenter (זה לא Cinema Studio רגיל אלא Soul-locked).

**דורשים אישור מפורש לפני שימוש**:
- `seedance_2_0` — אם רוצים lip-sync דיבור native (יותר חזק כשהקריינות והוידאו מאותו מקור)
- `veo_3_1` — לקולנועי איכותי
- `sora_2` — לריאליזם, 12 שניות
- `cinema_studio_3_5` — MCSLA built-in

### C — Camera
תנועת המצלמה והגדרות:
- **Static** (סטטית): מצלמה לא זזה
- **Handheld** (רגליים): קצת רעידות, אותנטי
- **Dolly-in/out**: זוחלת פנימה/החוצה לאט
- **Pan left/right**: סיבוב אופקי
- **Tilt up/down**: סיבוב אנכי
- **Drone / aerial**: מבט-על
- **Tracking**: עוקבת אחרי הנושא
- **Crane**: זווית גבוהה

### S — Subject
מי / מה במרכז הפריים:
- אדם (description ברור או Soul ID)
- מוצר (תיאור מדויק)
- מקום
- אובייקט מופשט

### L — Look
תאורה, צבע, mood:
- **תאורה**: golden hour / blue hour / soft window light / harsh studio / neon noir
- **פלטה**: warm tones / cool tones / monochrome / desaturated / saturated
- **Mood**: dramatic / dreamy / documentary / commercial / cinematic

### A — Action
מה קורה — תנועה ופעולה:
- מה הנושא עושה
- מהירות התנועה
- אירועים בתוך השוט

---

## מתכון 1: UGC presenter עם מוצר

```
M: kling_3_0
C: handheld eye-level, slight shake, natural feel
S: <Soul ID> מחזיק את <מוצר>, פרזנטר אינסטה
L: תאורת חלון רכה משמאל, צבעים חמים, אסתטיקת אינסטה
A: מסתכל למצלמה, מציג את המוצר, מסתובב 90°, חיוך
Voiceover (חיצוני, ElevenLabs): <סקריפט עברית 30s, מורכב בעריכה>
Duration: 15s
```

> **הערה**: אין lip-sync ב-kling_3_0. הוידאו דמום או עם cap לא-דיברתי. הקריינות מורכבת בעריכה (CapCut). אם רוצים lip-sync native — לבקש אישור לעבור ל-`seedance_2_0`.

---

## מתכון 2: Cinematic product showcase

```
M: kling_3_0
C: dolly-in slow, eye-level, smooth
S: <מוצר> על משטח רפלקטיבי, רקע נקי
L: תאורה דרמטית, מקור אור עליון, צללים עמוקים, מעבר מחם לקריר
A: סיבוב 360° של המוצר תוך כדי dolly-in, light flare ב-2 השניות האחרונות
Duration: 8s
```

> אם רוצים את האיכות הקולנועית של Veo 3.1 — לבקש אישור.

---

## מתכון 3: Lifestyle hero

```
M: kling_3_0
C: tracking, follows subject, mid-shot
S: אישה ב-30+ הולכת ברחוב עירוני, מחזיקה <מוצר>
L: golden hour, חם, סופט, תאורת פנים מ-bounce
A: הולכת לכיוון מצלמה, מסתכלת הצידה, חיוך, קלוז-אפ של המוצר ביד
Duration: 10s
```

---

## מתכון 4: Conceptual / surreal

```
M: kling_3_0
C: static, low-angle, hero composition
S: <מוצר> מרחף באוויר במרכז סצנה
L: סוריאליסטי, צבעים רוויים, light bloom, dreamy
A: המוצר מסתובב לאט, אובייקטים זעירים מקיפים אותו, רעידה דקה
Duration: 6s
```

---

## מתכון 5: Soul ID — talking head

```
M: kling_3_0 + soul reference_id (chained)
C: static medium close-up, slight push-in (4%)
S: <Soul reference_id>, יושב על כיסא, רקע מטושטש
L: תאורת window key + soft fill, צבעים נטרליים, look UGC professional
A: מסתכל למצלמה, מחוות פנים מינימליות, breaks eye contact ב-frame 5
Voiceover (חיצוני): <סקריפט בעברית, מורכב בעריכה>
Duration: 10s
```

> אם רוצים lip-sync אמיתי בעברית במקום voiceover על וידאו דמום — לבקש אישור לעבור ל-`seedance_2_0` או `soul_cinema_studio`.

---

## מתכון 6: Before/After

```
M: kling_3_0
C: static, eye-level, identical framing
S: אותו מקום / אדם / חפץ — "לפני" ב-3 שניות ראשונות, "אחרי" ב-3 הבאות
L: לפני: cool, desaturated, dimm. אחרי: warm, saturated, bright
A: split על second 3 עם wipe transition
Duration: 6s
```

---

## טיפים לפרומפט מנצח

1. **בעברית או באנגלית?** — הפרומפט עצמו לרוב באנגלית (מה שהמודל מבין יותר טוב). הקריינות בעברית.

2. **תיאור ספציפי > מילים גדולות**. "שיער כתום עם פסים בלונדיניים שמכסים חצי פנים" עדיף על "אישה יפה".

3. **תיאור הפנים בקצרה** אם לא משתמשים ב-Soul ID — אחרת הפנים משתנות בין שוטים.

4. **מצלמה ראשונה, נושא שני**. תמיד קודם להגדיר את המצלמה — זה המסגרת.

5. **Length matters**. וידאו 6 שניות יותר חד מ-15 ש'. תכנון נכון = פחות סבל.

6. **לתעד מה שעבד** ב-`BRAND/prompt-library.md`.

---

## להימנע

- **תיאור איך מצלמה זזה ב-3 דרכים שונות** — בלבול. בחר אחד.
- **action כלאיים**: "רוקד וגם רץ וגם חוצה רחוב" — תוצאה יוצאת מבולגנת.
- **רקע מורכב מדי** — אם לא הכרחי, רקע נקי = פלט יציב.
- **prompts ארוכים מדי**. 60-100 מילים בדרך כלל מספיק.

---

## קישורים שימושיים

- [Higgsfield Cinema Studio Documentation](https://higgsfield.ai/cinema-studio)
- [OSideMedia Cinema Studio Skill](https://github.com/OSideMedia/higgsfield-ai-prompt-skill) — 20 sub-skills מתקדמים
