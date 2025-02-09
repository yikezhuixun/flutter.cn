---
title: Set up an editor
title: 编辑工具设定
description: Configuring an IDE for Flutter.
description: 为 Flutter 配置 IDE 环境。
tags: Flutter安装,Flutter起步教程
keywords: Flutter编辑工具,IDE配置
prev:
  title: Install
  title: 安装和环境配置
  path: /docs/get-started/install
next:
  title: Test drive
  title: 开发体验初探
  path: /docs/get-started/test-drive
toc: false
---

You can build apps with Flutter using any text editor
combined with Flutter's command-line tools.
However, we recommend using one of our editor
plugins for an even better experience.
These plugins provide you with code completion, syntax
highlighting, widget editing assists, run & debug support, and more.

你可以使用任意文本编辑器，结合我们的命令行工具来开发 Flutter 应用。
然而，我们推荐使用我们的编辑器插件以获取更好的开发体验。这些插件提供了代码补全、
代码高亮、widget 辅助编辑的功能，以及为项目的运行和调试提供支持等。

Use the following steps to add an editor plugin for VS Code,
Android Studio, IntelliJ, or Emacs.
If you want to use a different editor,
that's OK, skip ahead to the [next step: Test drive][].

参考以下步骤为 VS Code、Android Studio、IntelliJ 或者 Emacs 添加编辑器插件。
如果你想使用其他的编辑器，请直接打开
[下一节: 开发体验初探][next step: Test drive]，
来查看使用其他文本编辑器配合命令行工具来创建和运行 Flutter 应用。

{% comment %} Nav tabs {% endcomment -%}
<ul class="nav nav-tabs" id="editor-setup" role="tablist">
  <li class="nav-item">
    <a class="nav-link active" id="vscode-tab" href="#vscode" role="tab" aria-controls="vscode" aria-selected="true">Visual Studio Code</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" id="androidstudio-tab" href="#androidstudio" role="tab" aria-controls="androidstudio" aria-selected="false">Android Studio 和 IntelliJ</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" id="emacs-tab" href="#emacs" role="tab" aria-controls="emacs" aria-selected="false">Emacs</a>
  </li>
</ul>

{% comment %} Tab panes {% endcomment -%}
<div class="tab-content">
<div class="tab-pane active" id="vscode" role="tabpanel" aria-labelledby="vscode-tab" markdown="1">

## Install VS Code

## 安装 VS Code

VS Code is a lightweight editor with complete Flutter
app execution and debug support.

VS Code 是一个可以运行和调试 Flutter 的轻量级编辑器。

* [VS Code][], latest stable version

  [VS Code][]，最新稳定版本

## Install the Flutter and Dart plugins

## 安装 Flutter 和 Dart 插件

 1. Start VS Code.

    打开 VS Code。

 1. Invoke **View > Command Palette...**.

    打开 **View > Command Palette...**。

 1. Type "install", and select
    **Extensions: Install Extensions**.

    输入「install」，然后选择
    **Extensions: Install Extensions**。

 1. Type "flutter" in the extensions search field,
    select **Flutter** in the list, and click **Install**.
    This also installs the required Dart plugin.

    在扩展搜索输入框中输入「flutter」，然后在列表中选择 **Flutter** 并单击 **Install**。
    此过程中会自动安装必需的 Dart 插件。

 1. Click **Reload to Activate** to reload VS Code.

    点击 **Reload to Activate** 以重新启动 VS Code。

## Validate your setup with the Flutter Doctor

## 通过 Flutter Doctor 命令验证是否安装成功

 1. Invoke **View > Command Palette...**.

    打开 **View > Command Palette...**。

 1. Type "doctor", and select the
    **Flutter: Run Flutter Doctor**.

    输入 "doctor"，选择
    **Flutter: Run Flutter Doctor**。

 1. Review the output in the **OUTPUT** pane for any issues.
    Make sure to select Flutter from the dropdown
    in the different Output Options.

    打开 **OUTPUT** 面板查看是否有错误，
    确保在不同的输出选项 (Output Options) 
    的下拉列表中选择了 Flutter。

</div>
<div class="tab-pane" id="androidstudio" role="tabpanel" aria-labelledby="androidstudio-tab" markdown="1">

## Install Android Studio

## 安装 Android Studio

Android Studio offers a complete,
integrated IDE experience for Flutter.

Android Studio 为 Flutter 提供了一个完整的集成开发环境。

* [Android Studio][], version 2020.3.1 (Arctic Fox) or later

  [Android Studio](https://developer.android.google.cn/studio)，2020.3.1 (Arctic Fox) 或之后的版本

Alternatively, you can also use IntelliJ:

同时, 你也可以使用 IntelliJ：

* [IntelliJ IDEA Community][], version 2021.2 or later

  [IntelliJ IDEA Community][]，2021.2 或之后的版本

* [IntelliJ IDEA Ultimate][], version 2021.2 or later

  [IntelliJ IDEA Ultimate][]，2021.2 或之后的版本

## Install the Flutter and Dart plugins

## 安装 Flutter 和 Dart 插件

The installation instructions vary by platform.

请参考下面不同平台的安装指南：

### Mac

Use the following instructions for macos:

安装过程如下：

 1.  Start Android Studio.
    
     打开 Android Studio。

 1. Open plugin preferences (**Preferences > Plugins** as of
     v3.6.3.0 or later).

    打开插件设置（在 v3.6.3.0 以上的系统打开 **Preferences > Plugins**）。

 1. Select the Flutter plugin and
     click **Install**.

    然后选择 Flutter 插件并点击 **安装**。

 1. Click **Yes** when prompted to install the Dart plugin.

    当弹出安装 Dart 插件提示时，点击 **Yes**。

 1. Click **Restart** when prompted.

    当弹出重新启动提示时，点击 **Restart**。

### Linux or Windows

### Linux 或者 Windows 平台

Use the following instructions for Linux or Windows:

参考使用下面介绍的步骤：

   1. Open plugin preferences (**File > Settings > Plugins**).

      打开插件偏好设置 (位于 **File > Settings > Plugins**)

   1. Select **Marketplace**,  select the Flutter plugin and click
      **Install**.

      选择 **Marketplace (扩展商店)**，选择 Flutter plugin
      然后点击 **Install (安装)**。

</div>
<div class="tab-pane" id="emacs" role="tabpanel" aria-labelledby="emacs-tab" markdown="1">

## Install Emacs

## 安装 Emacs 编辑器

Emacs is a lightweight editor with support for Flutter and Dart.

Emacs 是一个轻量级的编辑器，支持 Flutter 和 Dart。

* [Emacs][], latest stable version

  最新版本的 [Emacs][] 编辑器。

## Install the lsp-dart package

## 安装 lsp-dart 这个 package

For information on how to install and use the package,
see the [lsp-dart documentation][].

关于如何安装和使用 lsp-dart 这个 package，可以查看
[lsp-dart 文档][lsp-dart documentation]。

</div>
</div>{% comment %} End: Tab panes. {% endcomment -%}


[Android Studio]: {{site.android-dev}}/studio
[IntelliJ IDEA Community]: https://www.jetbrains.com/idea/download/
[IntelliJ IDEA Ultimate]: https://www.jetbrains.com/idea/download/
[next step: Test drive]: {{site.url}}/get-started/test-drive
[VS Code]: https://code.visualstudio.com/
[Emacs]: https://www.gnu.org/software/emacs/download.html
[lsp-dart documentation]: https://emacs-lsp.github.io/lsp-dart/
