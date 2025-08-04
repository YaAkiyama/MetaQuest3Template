# Meta Quest 3 Unity VR Template

**Meta Quest 3 Unity VR開発環境テンプレート - Unity MCP + GitHub MCP Claude連携**

## 🎯 プロジェクト概要

このプロジェクトは、Meta Quest 3 での VR 開発を効率化するための統合開発環境テンプレートです。Unity MCP と GitHub MCP を活用した Claude 連携により、AI 支援による開発フローを実現します。

## 🛠️ 技術スタック

- **Unity**: 2022.3.62f1 LTS (Universal Render Pipeline)
- **XR Plugin**: OpenXR + Meta Quest Support  
- **Target Platform**: Android (Meta Quest 3)
- **Development Tools**: Unity MCP + GitHub MCP + Claude AI

## 📋 開発環境

### 前提条件
- Windows 10 (64-bit)
- Unity 2022.3.62f1 LTS
- Android Studio Narwhal 2025.1.2+
- Meta Quest 3 (開発者モード有効)
- Claude Desktop (Unity MCP + GitHub MCP 設定済み)

### 環境構築状況
- ✅ **Phase 1**: 基本開発ツール環境構築完了
- ✅ **Phase 2**: Unity MCP + GitHub連携セットアップ完了  
- 🔄 **Phase 3**: Meta Quest 3 開発環境セットアップ（進行中）

## 🚀 セットアップ手順

### 1. リポジトリクローン
```bash
git clone https://github.com/YaAkiyama/MetaQuest3Template.git
cd MetaQuest3Template
```

### 2. Unity プロジェクト開く
- Unity Hub で本プロジェクトを開く
- Unity 2022.3.62f1 LTS を使用

### 3. 必須パッケージ確認
- Meta OpenXR
- XR Interaction Toolkit  
- Android Logcat
- Unity MCP Bridge

### 4. Platform 設定
- Build Settings → Android に切り替え
- XR Plug-in Management → OpenXR + Meta Quest Support 有効

## 🔧 Unity MCP 連携機能

Claude Desktop との連携により以下が可能：

- **自動スクリプト生成**: VR インタラクション コード生成
- **デバッグ支援**: Console ログ取得・エラー解析
- **プロジェクト管理**: Unity Editor メニュー実行
- **GitHub 連携**: Issue 管理・PR 自動化

## 📱 Meta Quest 3 開発

### デバイス設定
1. Meta Quest 3 開発者モード有効化
2. USB デバッグ許可
3. ADB 接続確認: `adb devices`

### ビルド・テスト
```bash
# Unity Editor
File → Build Settings → Build and Run
```

## 🎮 VR テンプレート機能（予定）

- VR レーザーポインター システム
- World Space UI パネル
- XR Interaction System 統合
- Quest 3 最適化設定

## 📚 関連ドキュメント

- [Meta Quest 3 Unity VR開発環境完全セットアップ手順書](./docs/setup-guide.md)
- [Unity MCP 活用ガイド](./docs/unity-mcp-guide.md)
- [VR 開発ベストプラクティス](./docs/vr-best-practices.md)

## 🤝 開発フロー

1. **Claude で機能設計**: 「VR UI システムを設計して」
2. **自動コード生成**: Unity MCP 経由でスクリプト作成
3. **実機テスト**: Quest 3 でのビルド・検証
4. **GitHub 管理**: 変更履歴・Issue トラッキング

## 📊 パフォーマンス目標

- **フレームレート**: 90 FPS (Quest 3)
- **Draw Call**: 150以下
- **ポリゴン数**: 100k以下 (同時表示)
- **テクスチャメモリ**: 1GB以下

## 🎯 ロードマップ

- [x] Unity MCP + GitHub 環境構築
- [ ] Meta Quest 3 実機開発環境
- [ ] VR レーザーポインター テンプレート
- [ ] Quest 3 最適化設定
- [ ] CI/CD パイプライン構築

## 📄 ライセンス

MIT License

## 🔗 リンク

- [Meta Quest Developer Hub](https://developers.meta.com/horizon/downloads/)
- [Unity MCP Bridge](https://github.com/justinpbarnett/unity-mcp)
- [Claude Desktop](https://claude.ai/download)

---

**作成日**: 2025年8月4日  
**最終更新**: Phase 2 完了時点  
**Next**: Phase 3 - Meta Quest 3 開発環境セットアップ