---
tags:
  - instructor-manual
  - evergreen
  - VC1
  - version-control
last_modified: 2025-04-21
---

> [!tldr] TL;DR • Instructor Quick‑Start  
> - **Guiding Principles** – Kindness, clarity, share‑ability. Small iterations beat perfect prose. [[#Guiding Principles]]  
> - **Active‑Learning Pillars** – Do, discuss, teach. [[#Teaching Philosophy]]  
> - **Possible Techniques** – Debug Bingo, driver‑navigator pairing, 3‑minute silent debug drills. [[#Classroom Techniques]]  
> - **Cultural Tips** – Offer 30 sec thinking time & soften direct questions with “もしよければ”.  
> - **Contribute** – Fork → edit → MR; log changes in **[[99 Changelog]]**.

---

## Table of Contents
1. [[#Guiding Principles|Guiding Principles]]  
2. [[#How to Contribute|How to Contribute]]  
3. [[#Teaching Philosophy|Teaching Philosophy]]  
4. [[#Classroom Techniques|Classroom Techniques]]  

---

## Guiding Principles
*Kindness, clarity, share‑ability.* Small, incremental improvements beat perfect prose that never ships.  
*親切・明確・共有可能* がモットー。完璧を目指すより、小さな改善を積み重ねましょう。

> [!tip] Quick Win  
> Treat docs like code—branch, PR, review.  
> ドキュメントもコードと同じく「ブランチ→PR→レビュー」で管理しましょう。 

## Teaching Philosophy 
### Active‑Learning Pillars
Students learn by **doing**, **discussing**, and **teaching**. Code‑alongs, pair explanations, and micro‑projects turn passive listeners into engaged problem‑solvers.  

学習者は **実践**・**対話**・**教えること** で深く学びます。コーディング実演、ペア解説、マイクロプロジェクトが受動的な聴講者を能動的な問題解決者へと変えます。

> [!summary] Ethos • Pathos • Logos – Why They Work  
>
> - **Ethos (Credibility)** – Students trust instructors who show expertise (live debugging, industry anecdotes). Trust lowers cognitive load, so learners process new syntax more easily.  
> - **Pathos (Emotion)** – A humorous analogy or personal story triggers dopamine, increasing attention and long‑term memory—crucial when abstract concepts (e.g., recursion) feel intimidating.  
> - **Logos (Logic)** – Step‑by‑step reasoning or a whiteboard trace satisfies the brain’s need for coherence, reinforcing mental models of program flow.  
>  
>
> - **エトス（信頼）** – 講師のデバッグ実演や実務経験の共有が信頼を生み、認知負荷を下げて新しい構文を理解しやすくします。  
> - **パトス（感情）** – ユーモアや体験談はドーパミンを促し、注意力と記憶保持を高めます。再帰など抽象的な概念に効果的。  
> - **ロゴス（論理）** – 手順を可視化したホワイトボード説明は脳が求める一貫性を満たし、プログラムの流れを強固なメンタルモデルとして定着させます。  
> - > [!suggestion] Share Teaching Anecdotes  
>  Instructors are encouraged to share a real‑world story where using ethos, pathos, or logos noticeably helped students grasp a concept. Adding these to a shared “Ethos/Pathos/Logos Examples” section builds a practical reference that future instructors can draw from when preparing lessons or troubleshooting engagement issues.  
>  エトス・パトス・ロゴスを活用して学習者の理解が深まった実体験を、ぜひ共有してください。共有ノートの「Ethos/Pathos/Logos Examples」セクションに追加することで、今後の講師が授業準備や関心を引き出す工夫を考える際の実践的な参考になります。
#### Ethos/Pathos/Logos Examples

> [!example]+ My story (Your Name)
> **Ethos (Credibility):**  
> [Briefly state your background, experience, or position that gives credibility—1–2 sentences.]
**Pathos (Emotion):**  
> [Describe an emotional moment, challenge, or feeling students might relate to—keep it human.]
**Logos (Logic):**  
> [Connect the experience to a clear insight, pattern, or strategy that others can apply.]

> [!example]+ My story (Naveed)  
> **Ethos (Credibility):**  
> I have an engineering degree. I’ve used Python for nearly 17 years. I’ve taught STEM for over 8 years. But I still study every week. Because what worked 5 years ago might not work tomorrow.  
>  
> **Pathos (Emotion):**  
> Sometimes I feel overwhelmed too—like I’m constantly chasing moving targets. But I’ve learned that **feeling behind** doesn’t mean you’re failing. It means you care enough to keep growing.  
>  
> **Logos (Logic):**  
> In tech, learning isn’t a phase—it’s a loop. The moment you stop, the field moves past you. That’s why we stay curious, stay uncomfortable, and keep iterating—just like in code.

#### Cultural Awareness
Direct questions may feel abrupt to some Japanese learners. Soften with “もしよければ” or give silent thinking time (30 sec) before calling on volunteers.  

率直な質問は日本人学習者には唐突に感じられる場合があります。「もしよければ」を添える、30秒の思考タイムを設けるなど配慮しましょう。  

> [!explainer] Why pause & predict?
>  Asking students to predict the next line of code before showing it activates deep thinking and improves memory (generation effect). Works in live lessons, videos, and self-paced LMS modules—with just 30–60 sec per prompt.  
> 
> 次のコード行を予想させてから表示することで、深く考え、記憶に残りやすくなります（生成効果）。ライブ授業・録画・LMS でも使え、1 回あたり 30～60 秒で実施できます。  
---

## Classroom Techniques 
### Ice‑Breakers  
**Version Control Bingo** — each square lists a common Git/GitLab mistake (e.g., `Wrong Branch`, `Merge Conflict`). Students mark squares as they occur during hands-on practice or demos.  

**バージョン管理ビンゴ** — 各マスに `Wrong Branch` や `Merge Conflict` など Git/GitLab のよくあるミスを記載。演習やデモ中に実際に起きたらマスをチェックします。

| **Wrong Branch**          | **Merge Conflict**        | **Forgot `git add`**          | **Pushed to `main`**  | **SSH Key Error**            |
| ------------------------- | ------------------------- | ----------------------------- | --------------------- | ---------------------------- |
| **Cloned Wrong Repo**     | **No Remote Set**         | **Free Space 🔧**             | **Staged Wrong File** | **`git pull` Failed**        |
| **Missing `.gitignore`**  | **Permission Denied**     | **Mistyped Branch Name**      | **Detached HEAD**     | **Wrong Commit Author**      |
| **Forgot to Pull First**  | **Rebase Went Wrong**     | **Force Pushed Accidentally** | **Forgot `git init`** | **History Diverged**         |
| **`.git` Folder Deleted** | **`git status` Confused** | **Commit Message Blank**      | **Used `--force`**    | **Staged but Didn't Commit** |

> [!tip] Quick Win – Why Bingo Works  
> Games lower stress, raise motivation, and create peer-driven learning moments. Version Control Bingo adds fun to error spotting and helps normalize mistakes as part of the process—especially effective in mixed-skill classes.  
> 
> ゲーム形式は緊張を和らげ、モチベーションを高め、仲間同士の学び合いを促進します。ビンゴを通してエラー発見を楽しみながら、失敗は成長の一部であることを自然に理解できます。特にレベル差のあるクラスに効果的です。

> [!action] Solicit Ice‑Breaker Ideas  
>Please propose at least two new ice‑breaker activities tailored to programming classes and add them below this section with brief instructions.  
>
> プログラミング授業に適した新しいアイスブレイク活動を、少なくとも2つ提案してください。簡単な実施手順とともに、このセクションの下に追加しましょう。
### Pair Programming
EN: Use the *Driver‑Navigator* rotation every 15 minutes. Encourage Japanese ↔ English pairing for language immersion.  
JA: 15分ごとに *ドライバー／ナビゲーター* を交代。日英ペアで言語シャワー効果を狙います。

> [!tip] Quick Win  
> EN: Hand students a timer; peer‑managed time boxes teach responsibility.  
> JA: タイマーを学生に渡し、時間管理を任せると主体性が育ちます。

### Code Reviews & Debug Drills
Alternate between quick code reviews and 3‑minute silent debug drills. Debrief by asking “What surprised you?”  
コードレビューと3分間の静かなデバッグ演習を交互に実施し、「何が意外だった？」と振り返りましょう.
