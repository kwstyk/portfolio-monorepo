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

## カテゴリ相関図 (Mermaid)

```mermaid
graph LR
  SB(SecurityBasics) --> NW(Network)
  NW --> OS(System)
  OS --> SD(SecureDev)
  SD --> SIEM(LogsSIEM)
  SIEM --> VM(VulnMgmt)
  VM --> Cloud(CloudSecurity)
  Cloud --> Ops(SecurityOps)
  Ops --> Gov(Governance
