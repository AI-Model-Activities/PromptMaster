# Prompt Master

Prompt Masterは、GoogleのGemini APIを活用してAIプロンプトを効率的に管理・強化するための、Python製デスクトップアプリケーションです。直感的なUIを通じて、プロンプトエンジニアリングのワークフローを加速させます。

## Features

* **プロンプト強化:** ベースとなるプロンプトを入力すると、Gemini APIがより構造的で高性能なプロンプトを生成します。
* **プロンプト管理:** 作成・強化したプロンプトの保存、ロード、更新、削除が可能です (CRUD)。
* **比較表示:** ベースプロンプトと強化後のプロンプトを並べて表示し、変更点を容易に確認できます。
* **お気に入り機能:** 重要なプロンプトを「お気に入り」としてマークし、素早くアクセスできます。
* **柔軟な設定:** 使用するGeminiモデルや、プロンプト強化のベースとなる「システムプロンプト」をGUIから柔軟に設定・変更できます。
* **便利な機能:** ワンクリックでのクリップボードコピー、プロンプトの入れ替え、1行形式への変換など、便利なユーティリティを備えています。

## Requirements

* Python 3.7 以上
* [Google APIキー](https://ai.google.dev/pricing)
* 以下のPythonライブラリ:
  * `customtkinter`
  * `google-generativeai`
  * `pyperclip`

## Installation

1. このリポジトリをクローンまたはダウンロードします。

    ```bash
    git clone https://github.com/your-username/prompt-master.git
    cd prompt-master
    ```

2. 必要なライブラリをインストールします。（`requirements.txt` を作成し、以下の内容を記述してください）

    **requirements.txt:**

    ```
    customtkinter
    google-generativeai
    pyperclip
    ```

    以下のコマンドでインストールします。

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. 以下のコマンドでアプリケーションを起動します。

    ```bash
    python main.py
    ```

2. 初回起動時に、`config.json` と `saved_prompts.json` がスクリプトと同じディレクトリに自動生成されます。

3. 左下の入力欄に、お持ちのGoogle APIキーを入力してください。キーは`config.json`に保存されます。

4. 左側の「ベースプロンプト」に、強化したいプロンプトを入力します。

5. 「プロンプトを強化」ボタンをクリックすると、右側に強化されたプロンプトが表示されます。

6. 「セーブ」ボタンでプロンプトを保存したり、「ロード」ボタンで過去に保存したプロンプトを一覧から呼び出すことができます。

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.