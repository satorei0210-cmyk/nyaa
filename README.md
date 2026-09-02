/* 全体設定 */
:root {
  --main-color: #e6e6fa; /* ラベンダーベース */
  --accent-color: #8a2be2; /* 深いラベンダー */
  --gold-color: #d4af37; /* 福のイメージ（ゴールド） */
  --text-color: #333333;
  --bg-color: #fcfbfe;
}

body {
  margin: 0;
  padding: 0;
  font-family: "Helvetica Neue", Arial, "Hiragino Kaku Gothic ProN", "Meiryo", sans-serif;
  color: var(--text-color);
  background-color: var(--bg-color);
  line-height: 1.6;
}

/* ヘッダー */
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #ffffff;
  border-bottom: 2px solid var(--main-color);
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  font-size: 1.4rem;
  font-weight: bold;
  color: var(--accent-color);
}

.nav a {
  margin-left: 1.5rem;
  text-decoration: none;
  color: var(--text-color);
  font-weight: 500;
}

/* メインビジュアル */
.hero {
  background: linear-gradient(135deg, #f3e8ff 0%, #e6e6fa 100%);
  padding: 4rem 1rem;
  text-align: center;
}

.badge {
  display: inline-block;
  background-color: #ffffff;
  color: var(--accent-color);
  border: 1px solid var(--accent-color);
  padding: 0.3rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  margin-bottom: 1rem;
}

.hero h1 {
  font-size: 2.2rem;
  color: #4a2e80;
  margin: 0.5rem 0;
}

/* セクション共通 */
.section {
  max-width: 800px;
  margin: 0 auto;
  padding: 3rem 1rem;
}

.bg-light {
  background-color: #f8f5fc;
}

h2 {
  text-align: center;
  color: #4a2e80;
  border-bottom: 2px solid var(--main-color);
  display: inline-block;
  padding-bottom: 0.3rem;
  margin-bottom: 2rem;
  width: 100%;
}

.card {
  background: #ffffff;
  padding: 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.05);
  border: 1px solid #f0e6ff;
}

/* 概要テーブル */
table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  padding: 0.8rem;
  text-align: left;
  border-bottom: 1px solid #eee;
}

th {
  width: 25%;
  color: var(--accent-color);
}

/* SNSボタン */
.sns-buttons {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-bottom: 1.5rem;
}

.btn {
  display: inline-block;
  padding: 0.8rem 1.8rem;
  border-radius: 25px;
  text-decoration: none;
  color: #ffffff;
  font-weight: bold;
}

.instagram { background-color: #e1306c; }
.x-twitter { background-color: #000000; }

.sns-embed, .map-placeholder {
  text-align: center;
  padding: 2rem;
  background-color: #f0f0f0;
  border-radius: 8px;
  color: #666;
}

/* 過去の開催アーカイブ */
.archive-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.archive-card {
  background: #ffffff;
  padding: 1rem;
  border-radius: 8px;
  border: 1px solid #eee;
}

.photo-placeholder {
  height: 150px;
  background-color: var(--main-color);
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 6px;
  color: #666;
}

/* フッター */
.footer {
  text-align: center;
  padding: 1.5rem;
  background-color: #4a2e80;
  color: #ffffff;
  font-size: 0.85rem;
}

/* スマホ対応 */
@media (max-width: 600px) {
  .header {
    flex-direction: column;
    gap: 0.5rem;
  }
  .nav a {
    margin: 0 0.5rem;
    font-size: 0.9rem;
  }
  th, td {
    display: block;
    width: 100%;
  }
  th {
    padding-bottom: 0.2rem;
  }
}
