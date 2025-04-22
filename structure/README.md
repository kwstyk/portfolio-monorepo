# Knowledge Structure

このポートフォリオの「Structure」レイヤーでは、10カテゴリの知識体系を整理し、学びの全体像を示します。

## カテゴリ一覧

1. セキュリティの基本知識  
2. ネットワーク知識  
3. OSとシステムの理解  
4. セキュア開発と脆弱性理解  
5. ログ分析とSIEM活用  
6. 脆弱性スキャニングと管理  
7. クラウドセキュリティ  
8. セキュリティ運用・CSIRT・SOC  
9. 法令・倫理・ガバナンス  
10. ソフトスキル・言語・継続力  

### 1. セキュリティの基本知識

**Why（なぜ学ぶのか）**  
- 情報セキュリティの土台となる概念（CIAトライアングルやAAA）を理解しておかないと、以降のすべての学び・実践が曖昧になってしまうため。  
- 組織やシステムに潜むリスクを正しく評価し、適切な対策を選択できるようになる。

**What（何を学ぶのか）**  
- CIAトライアングル（機密性, 完全性, 可用性）  
- AAAモデル（認証 Authentication / 認可 Authorization / アカウンティング Accounting）  
- 暗号化技術の基礎（対称鍵暗号, 公開鍵暗号, ハッシュ関数）  
- リスクマネジメント用語（脅威, 脆弱性, インパクト, リスク）  

**How（どうやって実践するか）**  
1. **TryHackMe “Intro to Cyber Security”** を Docker コンテナで再現  
   - `docker run --rm -it tryhackme/intro-to-cybersec bash`  
   - そこで出てくる簡易ラボ演習を自分で操作しながら、CIA や AAA の概念を確認する。  
2. **Markdown スライド資料の作成**  
   - 各概念（CIA, AAA, 暗号化, リスクマネジメント）をまとめた Markdown を Zenn 記事として公開。  
3. **Anki カード化**  
   - 学んだ用語と定義を Anki に登録し、毎日覚えられるようレビューを継続。  



## カテゴリ相関図 (Mermaid)

```mermaid
graph LR
  SB[Security Basics]       --> NW[Network]
  NW --> OS[System]
  OS --> SD[Secure Dev]
  SD --> SIEM[Logs SIEM]
  SIEM --> VM[Vuln Mgmt]
  VM --> CL[Cloud Security]
  CL --> OP[Security Ops]
  OP --> GV[Governance]

