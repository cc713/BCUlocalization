# Bulk Crap Uninstaller — Translation Guide

![License](https://img.shields.io/badge/license-Apache--2.0-blue.svg)
![Languages](https://img.shields.io/badge/languages-EN%20%7C%20中文-brightgreen.svg)

> Help translate BCU into your language.
> 帮助把 BCU 翻译成你的语言。

**[English](#english)** · **[简体中文](#简体中文)**

---

## English

### Table of contents

1. [Getting started](#getting-started)
2. [Translating the application](#translating-the-application)
3. [Translating the installer](#translating-the-installer)
4. [Finish](#finish)
5. [Things to keep in mind](#things-to-keep-in-mind)

### Getting started

1. Download the latest version of this translation tool: <https://github.com/HakanL/resxtranslator>
2. Open <https://github.com/Klocman/Bulk-Crap-Uninstaller/releases> and download the latest BCU Localisation Pack. Extract the zip somewhere safe.

### Translating the application

1. Run ResxTranslator, close the popup and click **File > Open directory**. Point it to the extracted `Files to translate` folder.
2. Click on any of the items in the left tree — it will open on the right. You need to translate all of those items; most are quite small.
   - You can use the **Missing translations** tab for a more convenient list of things left to translate. You might need to manually add your language to one of the files before this option becomes available.
3. Put the translation into the column marked with your language's code. For example, if you are translating to German, use the `de` column.
   - For a list of all language codes, click **Languages > Add > More Languages**. If possible, use only neutral languages.
   - If the column doesn't exist, click **Languages > Add > Your Code**. If your code is not available, click **More Languages**.

> [!TIP]
> If possible, use a more general locale. For example, try using `en` or `ru` instead of `en-GB` or `ru-RU`.

> [!NOTE]
> You can hide columns for different languages using the checkboxes below the list. This frees up screen space.

4. Once in a while, click **File > Save all modified** (or <kbd>Ctrl</kbd>+<kbd>S</kbd>) to save your work in case something crashes.
5. When done, save all changes and exit the translator.

### Translating the installer

1. When you are done translating inside ResxTranslator, open the `Files to translate\BulkCrapUninstaller\installer\scripts` folder.
2. Open the files in a text editor.
3. Look for the `[CustomMessages]` section.
4. Add a translation to each of the English entries there. The translated texts start with a short language code followed by a dot (for example `de.`, `pl.` or `nl.`).

For example, this is an English entry that needs to be translated:

```ini
InstallPortableTitle =Portable Installation
```

This is a German translation of this entry:

```ini
de.InstallPortableTitle =Tragbar Installation
```

> [!WARNING]
> Make sure that your translated text is not longer than the English text or other translations. If you see any items like `%n` or `%1`, leave them untouched in your translation. `%n` inserts a new line, while `%1`, `%2` etc. insert some text from the script.

5. Save changes to the original files.

### Finish

Compress the `Files to translate` folder you just modified into a `.zip` and send it back to me — I'll integrate it into the application.

If you don't have my e-mail address, use the contact form: <https://klocmansoftware.weebly.com/contact.html>

### Things to keep in mind

> [!IMPORTANT]
> Only translate `.resx` files with your language code (`filename.code.resx`). All other files will be ignored.

- Don't translate files named `Resources.resx`.
- In some texts you will find a `&` character, for example `&Help`. This character is used in menus to tell Windows which letter should be underlined when pressing <kbd>Alt</kbd>. The underlined character is used as a hotkey. To get a preview, try pressing <kbd>Alt</kbd> in any application with a standard menu bar to see what it looks like (BCU works too, of course).
- Try to keep your translations short and to the point. Try not to exceed the length of the original translation, especially on buttons and checkboxes — they generally will not reflow correctly and your translation could get clipped.

---

## 简体中文

### 目录

1. [准备工作](#准备工作)
2. [翻译应用程序](#翻译应用程序)
3. [翻译安装程序](#翻译安装程序)
4. [完成](#完成)
5. [注意事项](#注意事项)

### 准备工作

1. 下载最新版翻译工具：<https://github.com/HakanL/resxtranslator>
2. 打开 <https://github.com/Klocman/Bulk-Crap-Uninstaller/releases> 并下载最新的 BCU 本地化包（Localisation Pack）。把压缩包解压到安全的位置。

### 翻译应用程序

1. 运行 ResxTranslator，关闭弹窗，点击 **文件 > 打开目录**，指向解压出来的 `Files to translate` 文件夹。
2. 点击左侧树中的任意条目，它会在右侧打开。你需要翻译所有这些条目，其中大多数都很短。
   - 可以使用 **Missing translations**（缺失翻译）标签页，得到一份更便于处理的待翻译清单。启用该选项前，你可能需要先手动把语言添加到其中一个文件里。
3. 把译文填入以你的语言代码标记的列。例如，翻译成德语就使用 `de` 列。
   - 完整语言代码列表见 **语言 > 添加 > 更多语言**。如有可能，只使用中性语言。
   - 如果列不存在，点击 **语言 > 添加 > 你的代码**。如果你的代码不可用，点击 **更多语言**。

> [!TIP]
> 如有可能，请使用更通用的区域设置。例如用 `en` 或 `ru`，而不是 `en-GB` 或 `ru-RU`。

> [!NOTE]
> 可以用列表下方的复选框隐藏其他语言的列，从而腾出屏幕空间。

4. 时不时按 **文件 > 保存所有修改**（或 <kbd>Ctrl</kbd>+<kbd>S</kbd>）保存工作，以防程序崩溃。
5. 完成后保存所有更改并退出翻译工具。

### 翻译安装程序

1. 在 ResxTranslator 中翻译完成后，打开 `Files to translate\BulkCrapUninstaller\installer\scripts` 文件夹。
2. 用文本编辑器打开这些文件。
3. 找到 `[CustomMessages]` 段。
4. 你需要为其中每一条英文条目添加翻译。译文以简短的语言代码加点号开头（例如 `de.`、`pl.` 或 `nl.`）。

例如，下面是一条需要翻译的英文条目：

```ini
InstallPortableTitle =Portable Installation
```

对应的德语翻译是：

```ini
de.InstallPortableTitle =Tragbar Installation
```

> [!WARNING]
> 确保译文不比英文原文或其他译文更长。如果看到 `%n` 或 `%1` 之类的项，翻译时原样保留。`%n` 插入换行，`%1`、`%2` 等则插入脚本中的文本。

5. 保存对原始文件的更改。

### 完成

把修改后的 `Files to translate` 文件夹压缩成 `.zip` 发回给我，我会把它整合进应用程序。

如果没有我的邮箱地址，可以使用联系表单：<https://klocmansoftware.weebly.com/contact.html>

### 注意事项

> [!IMPORTANT]
> 只翻译与你的语言代码对应的 `.resx` 文件（`filename.code.resx`），其余文件都会被忽略。

- 不要翻译名为 `Resources.resx` 的文件。
- 有些文本中含有 `&` 字符，例如 `&Help`。该字符用于在菜单中告诉 Windows 按下 <kbd>Alt</kbd> 时应该给哪个字母加下划线，带下划线的字母即热键。想看效果，可以在任意带标准菜单栏的应用程序中按 <kbd>Alt</kbd>（当然，BCU 也可以）。
- 尽量让译文简短、直接。尽量不要超过原文长度，尤其是按钮和复选框上的文字——它们通常不会正确重排，译文可能被截断。