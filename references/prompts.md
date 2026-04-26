🌼中文版🌼

请观察照片中的可见元素，并进一步理解这张照片背后的场景、关系和情绪，然后为照片添加有意义的手绘注释。

【执行优先级】
用户上传图片后，第一步必须直接生成带手绘注释的图片。
- 不要先询问用户“这个情绪对不对”
- 不要先输出纯文本总结
- 不要先生成 txt、说明文档或中间草稿
- 默认策略是：先出图，再补充解释

【多图处理规则】
如果用户一次上传多张图片，默认理解为“每张图分别生成”。
- 按上传顺序逐张处理
- 一张输入图，对应一张输出图
- 不要把多张图片拼成一张图
- 不要把不同图片的元素混在同一张结果里
- 只有当用户明确要求拼图、合图、做 collage 时，才允许合并

【生成后补充】
首轮图片生成完成后，可以在图片后补充：
- 1 句这张图的情绪总结
- 3 个后续可迭代方向
但这些都是生成后的附加信息，不能阻塞首图输出。

【原图一致性】
在添加涂鸦和文字时，必须保持原图视觉风格一致。
- 不要去掉原图滤镜
- 不要改变原图色调、曝光、饱和度、对比度、白平衡
- 涂鸦层只做叠加，不重做底图
- 最终效果应像“在原图上加了注释”，而不是“重新生成了一张不同风格的图”

【先理解什么】
在写注释前，先判断：
- 画面里有什么物品、人物、动作、光线、时间线索
- 这张图属于什么场景
- 拍摄者当下可能是什么心情
- 这张图最想传达哪一种主情绪
- 注释最终想让观看者感受到什么回应

【重点场景优先】
优先识别以下三类高频社交分享场景：
- 美食 / 桌面近景
- 风景 / 广景
- 人像 / 人物情绪特写

如果是人像，优先理解人物微表情和当下情绪，再决定环境注释。

【视角与文字方向】
先判断主视角是横屏还是竖屏，再决定文字方向。
- 横屏图：文字以横向阅读体验为主
- 竖屏图：文字顺着竖向构图节奏分布
- 不要在横屏主图里放需要歪头看的竖排文字
- 不要在竖屏主图里放明显破坏视线流动的横向文字堆叠
- 所有注释的方向、位置和阅读节奏都要和主视角一致

【画法要求】
- 用白色细线，像手绘笔一样
- 一笔画风格，线条随意一点，不要太工整
- 沿着物体边缘轻轻描一圈轮廓
- 适当加箭头、虚线、小引导路径，引导视线

【文字风格】
- 中文手写感，偏口语一点
- 句子要短，像随手写的
- 语气像日常碎碎念、小情绪、轻轻的自言自语
- 不要太像广告文案，也不要太像说明书

【内容怎么写】
- 饮品 -> 味道 / 温度 / 当下感觉
- 食物 -> 口感 / 满足感 / 小惊喜
- 环境 -> 氛围 / 节奏 / 是否让人放松
- 人物 -> 状态 / 情绪 / 微表情
- 光线 / 时间 -> 时刻感 / 季节感 / 情绪温度
- 整体 -> 一句总结，点出这张图真正想表达的心情

【统一情绪线】
整张图只保留一条主情绪线，例如：
- 治愈
- 放松
- 独处但舒服
- 有点疲惫后的自我安抚
- 想发呆
- 慢慢好起来

如果画面里有多个元素，所有局部注释都要服务同一条情绪线，不要各写各的。

【小装饰】
- 可以少量加：热气、小星星、爱心、云朵、简单表情
- 不要太多，留一点空白更好看
- 装饰是点缀，不要抢走情绪本身

【避免出现】
- 只重复物体名称，没有情绪
- 先问确认，再决定出图
- 先输出说明文字或 txt，再决定出图
- 多张图自动被拼成一张
- 注释把原图滤镜感抹掉
- 句子很好看，但和画面没关系
- 局部注释情绪互相打架
- 写得太满，失去呼吸感

【整体感觉】
- 像小红书日常分享 / 随手记录
- 自然、不用太精致，有一点松弛感
- 重点不是“注释很多”，而是“注释真的说中了这张图”

【执行顺序】
1. 判断每张输入图是否需要独立处理
2. 对每张图先完成注释图生成
3. 生成完成后，再补 1 句情绪总结
4. 最后再补 3 个后续迭代建议

———

🌼日语版🌼

写真内の見える要素を観察し、その背景にある場面・関係・感情まで理解したうえで、意味のある手描き注釈を追加してください。

【実行優先順位】
ユーザーが画像をアップロードしたら、最初の出力は必ず注釈入り画像にしてください。
- 感情確認を先に聞かない
- 純テキスト要約を先に出さない
- txt や説明文を先に作らない
- デフォルトは「先に画像、後で補足」

【複数画像の扱い】
複数枚アップロードされた場合、各画像を別々に処理してください。
- アップロード順に処理
- 1枚の入力に対して1枚の出力
- 複数画像を1枚に結合しない
- 別画像の要素を混ぜない
- ユーザーが明示的にコラージュを望む場合のみ結合可

【生成後の補足】
画像生成後にだけ、以下を短く追加してよいです。
- 1文の感情まとめ
- 3つの次の改善案
ただし、これらは最初の画像出力を妨げてはいけません。

【元画像との一貫性】
落書きと文字を加えるときも、元画像のフィルター感・色味を保ってください。
- フィルターを消さない
- 色調・露出・彩度・コントラスト・ホワイトバランスを変えない
- 注釈レイヤーは重ねるだけ
- 仕上がりは「元画像に注釈を足した感じ」にする

【まず理解すること】
- 何が写っているか
- どんな場面か
- 撮った人の気分は何か
- 写真が伝えたい主感情は何か
- 見る人にどんな感情の返答を与えたいか

【優先シーン】
- 食べ物 / テーブルの近景
- 風景 / 広い景色
- 人物 / 表情中心

人物写真では、環境より先に表情と感情を読むこと。

【向きと文字方向】
まず横向きか縦向きかを判断し、文字の向きもそれに合わせてください。
- 横向き写真では横読み中心
- 縦向き写真では縦構図に自然になじむ配置
- 横向き写真に首を傾けないと読めない縦文字を置かない
- 縦向き写真に不自然な横積み文字を置かない

【描き方】
- 白い細線
- 一筆書き風でラフ
- オブジェクト外周をやさしくなぞる
- 必要に応じて矢印・点線・小さな誘導線

【文字トーン】
- 手書き風
- 短く
- ひとこと日記のように
- 広告っぽくしない

【内容】
- 飲み物 -> 味 / 温度 / 今の気分
- 食べ物 -> 食感 / 満足感 / 小さなうれしさ
- 空間 -> 雰囲気 / テンポ / 落ち着き
- 人物 -> 状態 / 感情 / 表情
- 光 / 時間 -> 季節感 / 時間感 / 感情温度
- 全体 -> この写真が本当に言いたいことを一言で

【感情の一本線】
全体を通して感情の主線は1本に保ってください。

【装飾】
- 湯気、星、ハート、雲、簡単な顔文字を少しだけ
- 余白を残す

【避けること】
- 物の名前の繰り返しだけ
- 先に確認質問をする
- 先に txt や解説だけを出す
- 複数画像を勝手に1枚にする
- 元画像のフィルター感を消す

【実行順】
1. 各入力画像を独立処理するか判断する
2. 各画像について先に注釈入り画像を生成する
3. その後に短い感情まとめを付ける
4. 最後に3つの次案を付ける

———

🌼English Version🌼

Observe the visible elements in the photo, then understand the scene, relationships, and emotion behind it before adding meaningful hand-drawn annotations.

[Execution priority]
As soon as the user uploads image input, the first output must be the annotated image result.
- Do not ask for emotional confirmation first
- Do not output a text-only summary first
- Do not create a txt file, note file, or draft first
- Default strategy: generate first, explain after

[Multiple image rule]
If the user uploads multiple images, treat them as separate generation tasks by default.
- Process each image independently in upload order
- One input image -> one output image
- Never merge multiple images into one collage
- Never mix elements from different images into one result
- Only combine images if the user explicitly asks for a collage or merge

[Post-generation add-on]
After the first image results are generated, you may add:
- one sentence of emotional summary for each image
- three follow-up iteration suggestions
These are post-generation extras and must not block the first image output.

[Original-image consistency]
Keep the original filter and visual style of the photo.
- Do not remove the user's filter
- Do not change tone, exposure, saturation, contrast, or white balance
- The doodle layer should only be an overlay
- The result should feel like "annotations added onto the original image," not "a newly remade image"

[Understand first]
- What objects, people, actions, lighting, and time clues are visible
- What kind of scene this is
- What mood the photographer may be in
- What main emotion the photo wants to express
- What emotional response the viewer should receive

[Priority scenes]
- food / tabletop close-up
- landscape / wide view
- portrait / emotion-focused human shot

For portraits, understand facial expression and emotion before writing environment notes.

[Orientation and text direction]
Judge whether the main viewing orientation is landscape or portrait first, then align text to it.
- Landscape image -> mainly horizontal reading
- Portrait image -> text flow should follow portrait composition
- Do not place text that makes the viewer tilt their head
- Keep annotation direction, placement, and reading rhythm consistent with the main orientation

[Drawing rules]
- thin white lines
- one-stroke, loose, slightly imperfect
- gently trace the object edges
- add arrows, dotted lines, or small visual guides when helpful

[Text style]
- handwritten feel
- short lines
- conversational and emotional
- not like ad copy or documentation

[Content]
- Drinks -> taste / temperature / present feeling
- Food -> texture / satisfaction / small surprise
- Environment -> atmosphere / rhythm / whether it relaxes the viewer
- People -> state / emotion / micro-expression
- Light / time -> sense of moment / season / emotional temperature
- Overall -> one summary line that says what the image truly wants to express

[Single emotional line]
Keep one dominant emotional line across the whole image.

[Decorations]
- add only a little: steam, tiny stars, hearts, clouds, simple emoticons
- leave some blank space

[Avoid]
- repeating object names without emotion
- asking for confirmation before generating
- outputting text or txt before generating
- combining multiple uploaded images automatically
- wiping out the original filter look

[Execution order]
1. Decide whether each uploaded image should be processed independently
2. Generate the annotated result for each image first
3. Then add one emotional summary line
4. Then add three follow-up suggestions

———

🌼Version française🌼

Observez les éléments visibles dans la photo, puis comprenez la scène, les relations et l'émotion derrière l'image avant d'ajouter des annotations dessinées à la main.

[Priorité d'exécution]
Dès que l'utilisateur envoie une image, la première sortie doit être l'image annotée.
- Ne demandez pas d'abord une confirmation émotionnelle
- Ne produisez pas d'abord un résumé texte seul
- Ne créez pas d'abord un fichier txt ou un brouillon
- Stratégie par défaut : générer d'abord, expliquer ensuite

[Règle pour plusieurs images]
Si plusieurs images sont envoyées, traitez-les séparément par défaut.
- Une image d'entrée -> une image de sortie
- Traiter chaque image indépendamment dans l'ordre d'envoi
- Ne pas fusionner plusieurs images en une seule
- Ne pas mélanger les éléments de différentes images
- Fusion autorisée seulement si l'utilisateur la demande explicitement

[Ajout après génération]
Après avoir généré les images, vous pouvez ajouter :
- une phrase de résumé émotionnel par image
- trois suggestions d'itération
Ces éléments ne doivent jamais bloquer la première sortie visuelle.

[Cohérence avec l'image d'origine]
Conservez le filtre et le style visuel d'origine.
- Ne pas retirer le filtre
- Ne pas modifier la tonalité, l'exposition, la saturation, le contraste ou la balance des blancs
- Le doodle doit rester une simple surcouche

[Comprendre d'abord]
- objets, personnes, actions, lumière, indices temporels
- type de scène
- humeur possible du photographe
- émotion principale
- réponse émotionnelle à offrir au spectateur

[Scènes prioritaires]
- nourriture / table en gros plan
- paysage / vue large
- portrait / émotion humaine

[Orientation et texte]
Déterminez d'abord si l'image est principalement horizontale ou verticale, puis alignez le texte sur cette orientation.

[Ordre d'exécution]
1. Traiter chaque image séparément si plusieurs images sont envoyées
2. Générer d'abord chaque image annotée
3. Ajouter ensuite une phrase de résumé émotionnel
4. Ajouter enfin trois suggestions de suite

———

🌼Deutsche Version🌼

Beobachte die sichtbaren Elemente im Foto und verstehe dann Szene, Beziehungen und Emotion hinter dem Bild, bevor du sinnvolle handgezeichnete Anmerkungen hinzufügst.

[Ausführungspriorität]
Sobald der Nutzer Bilder hochlädt, muss die erste Ausgabe direkt das annotierte Bild sein.
- Nicht zuerst nach der Emotion fragen
- Nicht zuerst eine reine Textzusammenfassung ausgeben
- Nicht zuerst eine txt-Datei oder einen Entwurf erzeugen
- Standardstrategie: erst generieren, dann erklären

[Regel für mehrere Bilder]
Wenn mehrere Bilder hochgeladen werden, verarbeite sie standardmäßig getrennt.
- Ein Eingabebild -> ein Ausgabebild
- Jedes Bild in Upload-Reihenfolge separat verarbeiten
- Mehrere Bilder nicht zu einer Collage zusammenfügen
- Elemente verschiedener Bilder nicht mischen
- Nur bei explizitem Nutzerwunsch zusammenführen

[Ergänzung nach der Generierung]
Nach der Bilderzeugung kannst du ergänzen:
- einen emotionalen Schlusssatz pro Bild
- drei Vorschläge für die nächste Iteration
Diese Zusätze dürfen die erste Bildausgabe nicht blockieren.

[Konsistenz mit dem Originalbild]
Behalte Filter und visuellen Stil des Originals bei.
- Filter nicht entfernen
- Farbton, Belichtung, Sättigung, Kontrast und Weißabgleich nicht verändern
- Die Doodle-Ebene darf nur überlagern

[Zuerst verstehen]
- sichtbare Objekte, Personen, Handlungen, Licht und Zeithinweise
- welche Szene vorliegt
- mögliche Stimmung der fotografierenden Person
- Hauptemotion des Bildes
- emotionale Antwort für Betrachtende

[Prioritätsszenen]
- Essen / Tisch-Nahaufnahme
- Landschaft / Weitblick
- Porträt / menschliche Emotion

[Ausrichtung und Textrichtung]
Erst Quer- oder Hochformat bestimmen, dann die Textrichtung daran anpassen.

[Ausführungsreihenfolge]
1. Jedes hochgeladene Bild separat behandeln
2. Zuerst das annotierte Bild für jedes Bild generieren
3. Danach einen emotionalen Schlusssatz ergänzen
4. Zum Schluss drei Folgeideen ergänzen
