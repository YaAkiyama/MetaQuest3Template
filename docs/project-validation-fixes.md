# Project Validation Issues 修正手順書

## 🚨 Critical Issues 解決

### 1. Color Space 設定修正
**問題**: `[OpenXR] Gamma Color Space is not supported when using OpenGLES`

**解決手順**:
```
Edit → Project Settings → Player → Android Settings
→ Other Settings → Rendering → Color Space = Linear
```

### 2. Android Architecture 設定修正  
**問題**: `[OpenXR] Only arm64 or x86_x64 is supported on Android with OpenXR`

**解決手順**:
```
Edit → Project Settings → Player → Android Settings
→ Other Settings → Target Architectures = ARM64 only
```

### 3. XR Hands Package インストール
**問題**: `[XR Interaction Toolkit] XR Hands package must be installed`

**解決手順**:
```
Window → Package Manager → Unity Registry
→ Search: "XR Hands" → Install
```

## ⚠️ Warning Issues 解決

### 4. InputSystem.XR.PoseControl 設定
**問題**: `[OpenXR] Switch to use InputSystem.XR.PoseControl`

**解決手順**:
```
Edit → Project Settings → XR Plug-in Management → OpenXR
→ Interaction Profiles → Add "OpenXR Interaction Profile"
```

### 5. StickControl Thumbsticks 設定
**問題**: `[OpenXR] Switch to use StickControl thumbsticks`

**解決手順**:
```
Window → Package Manager → XR Interaction Toolkit
→ Samples → Import "Starter Assets"
```

### 6. Screen Space Ambient Occlusion 最適化
**問題**: `[Meta Quest Support] Screen Space Ambient Occlusion performance issue`

**解決手順**:
```
Edit → Project Settings → Quality
→ Rendering → Screen Space Ambient Occlusion = Disabled
```

### 7. Run In Background 設定
**問題**: `[XR Plug-in Management] Run In Background setting`

**解決手順**:
```
Edit → Project Settings → Player → Android Settings
→ Resolution and Presentation → Run In Background = Enabled
```

### 8. Interaction Layer 31 設定
**問題**: `[XR Interaction Toolkit] Interaction Layer 31 for teleportation`

**解決手順**:
```
Edit → Project Settings → Tags and Layers
→ Layers → Add "Teleportation" to Layer 31
```

## 🔄 検証手順

1. 各設定変更後に `Apply` をクリック
2. `Edit → Project Settings → XR Plug-in Management → Project Validation`
3. `Fix All` または個別 `Fix` ボタンをクリック
4. 全てのエラー・警告が解決されることを確認

## 📊 修正完了チェックリスト

- [ ] Color Space: Linear
- [ ] Target Architecture: ARM64 only  
- [ ] XR Hands Package: Installed
- [ ] InputSystem.XR.PoseControl: 設定済み
- [ ] StickControl Thumbsticks: 設定済み
- [ ] Screen Space AO: Disabled
- [ ] Run In Background: Enabled
- [ ] Interaction Layer 31: Teleportation
- [ ] Project Validation: All Issues Fixed

---

**作成日**: 2025年8月6日  
**対象**: Meta Quest 3 Unity VR Template - Phase 7  
**前提**: Unity 2022.3.62f1 LTS + OpenXR + Meta Quest Support
