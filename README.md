# 倉島一也 / Kazuya Kurashima

塾の教室長。教育現場で 20 年以上、生徒・保護者・講師との面談は数千回規模。
現場の困りごとを、Claude Code で自分の手でツールにしています。

Director of a private tutoring school in Japan. 20+ years in education, thousands of meetings with students, parents and tutors.
I turn the problems I meet in my own classroom into tools, built with Claude Code.

## 作ってきたもの / What I've built

### LessonTrack — 自校で運用中 / in production at my school

プリント学習の記録アプリ。講師が採点済みの答案をスマホで撮ると、AI が教材・単元・点数を読み取り、講師が確認して保存します。自動採点ではなく、最終判断は講師です。

- **運用**：2026 年 3 月から自校で。2026 年 10 月現在、講師 3 名と自分、生徒 13 名。保護者向けの学習レポートを家庭に送付
- **更新**：7 か月で 18 リリース（0.1.0 → 0.13.3）
- **設計**：生徒の氏名を AI に送らない設計。氏名と学習データを構造的に分け、AI に渡すのは氏名を含まない答案データだけ。セキュリティレビューの記録をリポジトリに残している
- **技術**：Next.js 16 / React 19 / TypeScript / Supabase / Vercel。答案の読み取りは視覚モデル（Gemini API）。開発は Claude Code
- 自校で本番運用中のシステムのため、ソースのリポジトリは非公開

A learning-record app for a private tutoring school. A tutor photographs a graded worksheet, the AI reads the material, unit and score, and the tutor confirms and saves. In production since March 2026; as of October 2026 it is used by 3 tutors plus me and 13 students, with 18 releases in 7 months. Student names are not sent to the model by design: identity and learning data are kept separate, and the security review notes are documented in the repository. The repository is private because it is an internal system in production at my school.

### [which-model](https://github.com/kazuyakurashima/which-model) — 公開 / public

Claude Code 用の skill。やりたいことを伝えると、合うモデルと effort を理由つきで提案し、そのモデル向けに整えたプロンプトを渡します。2026 年 9 月、整えたプロンプトが素の依頼より役に立つかを条件を揃えて確かめましたが、この方法と規模では効果を確認できなかったので、開発を終了しました。結果と限界は README と記事に公開しています：[プロンプト最適化 OSS「which-model」の開発をやめた理由](https://www.linkedin.com/pulse/%E3%83%97%E3%83%AD%E3%83%B3%E3%83%97%E3%83%88%E6%9C%80%E9%81%A9%E5%8C%96oss-which-model%E3%81%AE%E9%96%8B%E7%99%BA%E3%82%92%E3%82%84%E3%82%81%E3%81%9F%E7%90%86%E7%94%B1-%E4%B8%80%E4%B9%9F-%E5%80%89%E5%B3%B6-utbxc/)（2026-10-02）

A Claude Code skill that recommends a model and effort level for your task, with reasons, and hands you a prompt tuned for it. In September 2026 I compared its prompts with plain requests under matched conditions. With this method and sample size I could not confirm a benefit, so I ended development. The results and limits are published in the README and in an [article (Japanese)](https://www.linkedin.com/pulse/%E3%83%97%E3%83%AD%E3%83%B3%E3%83%97%E3%83%88%E6%9C%80%E9%81%A9%E5%8C%96oss-which-model%E3%81%AE%E9%96%8B%E7%99%BA%E3%82%92%E3%82%84%E3%82%81%E3%81%9F%E7%90%86%E7%94%B1-%E4%B8%80%E4%B9%9F-%E5%80%89%E5%B3%B6-utbxc/).

### StudySpark — GLOBAL GEEK AUDITION 2025 Autumn 登壇 / presented at GGA 2025 Autumn

学習の「見える化」で、努力を続ける力に変える。子どもの学習履歴と努力を可視化し、AI コーチングと保護者向けダッシュボードで進捗を共有します。デジタルハリウッド「G's」のピッチイベント GLOBAL GEEK AUDITION 2025 Autumn（2025 年 11 月 17 日、SHIBUYA QWS）に登壇しました。ソースは非公開です。

Makes a child's study history and effort visible, and shares progress through AI coaching and a parent dashboard. Presented at GLOBAL GEEK AUDITION 2025 Autumn (Nov 17, 2025, SHIBUYA QWS), the pitch event of G's / Digital Hollywood. Source is private.

[プレスリリース / Press release](https://www.dhw.co.jp/press-release/20251030_gga2025autumn/) · [G's の紹介記事 / Feature on G's](https://g-s.dev/contents/productintro01/)

## いま / Now

**Built with Claude: Japan 2026**（Anthropic × Cerebral Valley、2026-11-02〜11-10、#claudejapan2026）に応募中。
作るのは、**面談する側（講師・コーチ）の振り返りを支える AI**。採点せず、本人の発言を原文で示し、次回試す一つの行動を決めます。

Applying to Built with Claude: Japan 2026 (Anthropic × Cerebral Valley). Building a reflection partner for the person *leading* the conversation: it cites your own words, never scores you, and helps you pick one thing to try next time.

## つながり / Links

X: [@gskaz224](https://x.com/gskaz224) · LinkedIn: [kazuya-kurashima](https://www.linkedin.com/in/kazuya-kurashima/)
