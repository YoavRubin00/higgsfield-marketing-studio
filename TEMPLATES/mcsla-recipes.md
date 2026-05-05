# MCSLA Recipes — נוסחאות Cinema Studio

> **MCSLA** = Model · Camera · Subject · Look · Action
> נוסחה רשמית של Higgsfield ל-Cinema Studio. הופכת פרומפט חלש לפלט מקצועי.
> ככל שכל ה-5 ברורים — הפלט יציב יותר.

---

## הסבר ה-5 רכיבים

### M — Model
איזה מודל וידאו של Higgsfield. בחירה משפיעה על הסגנון:
- `seedance_2_0` — UGC עם lip-sync טבעי, ספיש + תמונה במעבר אחד
- `kling_3_0` — motion control גבוה, frame-by-frame, action sequences
- `veo_3_1` — קולנועי איכותי, צבע עשיר
- `sora_2` — ריאליזם, 12 שניות, 1080p
- `cinema_studio_3_5` — מובנה עם MCSLA built-in
- `soul_cinema_studio` — Soul ID + Cinema Studio = דמות עקבית קולנועית

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
M: seedance_2_0
C: handheld eye-level, slight shake, natural feel
S: <Soul ID> מחזיק את <מוצר>, פרזנטר אינסטה
L: תאורת חלון רכה משמאל, צבעים חמים, אסתטיקת אינסטה
A: מסתכל למצלמה, מציג את המוצר, מסתובב 90°, חיוך
Voiceover: <סקריפט עברית 30s>
Duration: 15s
```

---

## מתכון 2: Cinematic product showcase

```
M: veo_3_1 או cinema_studio_3_5
C: dolly-in slow, eye-level, smooth
S: <מוצר> על משטח רפלקטיבי, רקע נקי
L: תאורה דרמטית, מקור אור עליון, צללים עמוקים, מעבר מחם לקריר
A: סיבוב 360° של המוצר תוך כדי dolly-in, light flare ב-2 השניות האחרונות
Duration: 8s
```

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
M: soul_cinema_studio
C: static medium close-up, slight push-in (4%)
S: <Soul reference_id>, יושב על כיסא, רקע מטושטש
L: תאורת window key + soft fill, צבעים נטרליים, look UGC professional
A: מסתכל למצלמה, מדבר טבעי, מחוות יד מינימליות, breaks eye contact ב-frame 5
Voiceover: <סקריפט>
Duration: 10s
```

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
